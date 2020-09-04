<template>
    <div>
   <h1>{{ title }}</h1>
   <n-link to = "/">home</n-link>
    </div>
</template>

<script>
    export default {
        // data() {
        //     return{
        //         title : 'ABOUT'
        //     }
        // },
       asyncData(){
           return{
               title : 'About'
               
           }
       },
       head() {
           return{
               title : 'about',
                script : [
                   { src : '/about.js'}
                ],
               meta : [
                   { hid : 'description',
                    name : 'description',
                    content : 'my amezing about page' 
                   }
                ]   

               
           }
       }
        
    }
</script>

<style lang="scss" scoped>

</style>