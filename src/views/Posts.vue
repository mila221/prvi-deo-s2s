<template>
    <div>
       <v-parallax height="200" src="https://cdn.vuetifyjs.com/images/parallax/material.jpg"> 

            <v-row justify="center" align="center">
                    
                    <v-col cols="11" sm="6">
                    <h1 class="text-center">Posts stranica</h1>
                    <v-text-field v-model="search" prepend-inner-icon="mdi-magnify" solo label="Pretrazi..."></v-text-field>
                    {{ search }}
                    </v-col>
                    
            </v-row>         
     </v-parallax>

<v-row justify="center" align="center">
    <v-col sm="6">
    <v-card v-for="post in filteredPosts" :key="post.id">
        <PostPreview :post="post" />
         
    </v-card>
    </v-col>

</v-row>

    

    </div>
</template>


<script>
import PostPreview from '../components/PostPreview'
import axios from 'axios'

export default {
    components: {
        PostPreview
    },
    data(){
        return{
            posts: [],
            search: '',
            
        }
    },
    created(){
        axios
            .get('https://jsonplaceholder.typicode.com/posts')
            .then(response=>{
                this.posts=response.data
                this.posts.splice(0,80)
            })
    },
    computed: {
        filteredPosts: function(){
            return this.posts.filter((post) => {
                return post.title.match(this.search)
            } )
        } 
    },
}
</script>
