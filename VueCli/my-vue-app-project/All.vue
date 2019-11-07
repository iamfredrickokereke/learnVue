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
                {name : 'fred', status: true},
                {name : 'eddna', status: false},
                {name : 'mary', status: true},
                {name : 'miracle', status: false}
            ]
        }
    }
}
</script>

<style>

</style>