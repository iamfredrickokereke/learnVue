<template>
    <div id="all-friends">
        <h1>All Friends</h1>
        <div v-for="(friend, index) in friends" :key="index">
            <span @click="unFriend(friend.name)">{{friend.name}}</span>
        </div>
    </div>
</template>
<script>
export default {
    name:'Friends',
    props: ['friends'],
    data(){
        return{
            

        }
    },

    methods:{
        unFriend(name){
            this.$emit('delete', {name})
        }
    }
}
</script>

<style>

</style>