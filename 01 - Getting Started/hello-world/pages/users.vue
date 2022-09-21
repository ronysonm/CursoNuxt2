<template>
    <div>
        <h1>This is a user page</h1>
        <div>
            <input type="text" v-model="userId">
            <button @click="onLoadUser">Load user</button>
        </div>
        <nuxt-child />
    </div>
</template>

<script>

export default {
    data() {
        return {
            userId: ''
        }
    },
    methods: {
        onLoadUser() {
            this.$router.push('/users/' + this.userId)
        }
    },
    layout: 'users'
}

</script>