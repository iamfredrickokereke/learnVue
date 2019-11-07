<template>
    <div id="all-friends">
        <h1>All Friends</h1>
        <div v-for="(friend, index) in friends" :key="index">
            <span>{{friend.name}}</span>
        </div>
    </div>
</template>
<script>
export default {
    name:'Friends',
    data(){
        return{
            

        }
    }
}
</script>

<style>

</style>