<template>
    <div id="online">
        <h1>Online Friends</h1>
        <div v-for="(friend, index) in friends" :key="index">
            <span v-if="friend.status">{{friend.name}}</span>
        </div>
    </div>
</template>

<script> 
    export default{
        name: 'online',
        data(){
             return{

                 

            ]
        }
        }
       
    }
</script>

<style>

</style>