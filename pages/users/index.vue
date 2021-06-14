<template>
    <div>
    <h1>The users view </h1>
    <input type="text" v-model="userId" />
    <button @click="onLoadUser">Load User</button>
    </div>
</template>


<script>
export default {
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