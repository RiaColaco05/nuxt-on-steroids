<template>
    <div>
    <h1>The users view </h1>
    <input type="text" v-model="userId" />
    <button @click="onLoadUser">Load User</button>
    <nuxt-child/>
    </div>
</template>
<script>
export default {
    layout: 'users',
    data() {
        return {
            userId: null
        }
    },
    methods: {
        onLoadUser(){
            this.$router.push({path : '/users/' + this.userId})
        }
    }
}
</script>