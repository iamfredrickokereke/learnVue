<template>
    <div id="all-friends">
        <div v-for="(friend, index) in friends" :key="index">
            <span>{{ friend.name }}</span>
        </div>
    </div>
</template>

<script>
export default {
    name: 'All',
    data(){
        return{
            friends: [
                {name : 'fred', status: 'online'},
                {name : 'eddna', status: 'offline'},
                {name : 'mary', status: 'online'},
                {name : 'miracle', status: 'offline'}
            ]
        }
    }
}
</script>

<style>

</style>