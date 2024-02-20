<template>
  <div>
    <h1>This is a users page</h1>
    <input type="text" v-model="userId" />
    <button @click="onLoadUser">Load User</button>
    <!-- the below points to the /users file structure. These are called nested routes -->
    <nuxt-child />
  </div>
</template>

<script>
export default {
  data() {
    return {
      userId: "",
    };
  },
  methods: {
    onLoadUser() {
      this.$router.push("/users/" + this.userId);
    },
  },
  layout: "users",
};
</script>