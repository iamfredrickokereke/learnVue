<template>
    <div id="online">
        <div v-for="(friend, index) in friends" :key="index">
            {{friend.status}}
        </div>
    </div>
</template>

<script> 
    export default{
        name: 'online',
        data(){
             return{

                 friends:[
                     
                    {name : 'fred', status : true},
                    {name : 'emma', status : true},
                    {name : 'charles', status : false},
                    {name : 'nonso', status : false}

            ]
        }
        }
       
    }
</script>

<style>

</style>