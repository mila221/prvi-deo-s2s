<template>
    <div>
        <v-card-title>{{ post.title }}</v-card-title>
        <v-card-text>
            <h3>Author name</h3>
            {{ post.body }}
        </v-card-text>
        <v-card-actions>
            <v-spacer></v-spacer>
            <v-btn icon @click="favorite()">
                <v-icon  :class="{active: Isactive}">mdi-heart</v-icon>
            </v-btn>
        </v-card-actions>
    </div>
</template>
<script>
export default {
    props: ['post'],
    data(){
        return{
            Isactive: false
        }
    },
     methods: {
        favorite(){
            this.Isactive= !this.Isactive
        }
    }
}
</script>
<style scoped>
.active.mdi-heart{
    color: red;
}
</style>