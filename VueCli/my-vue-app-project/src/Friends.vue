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