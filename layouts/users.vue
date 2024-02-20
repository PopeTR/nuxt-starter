// Custom layout for users which has been linked to the relevant pages in the layouts part of the script tag
<template>
  <div>
    <Header />
    <header>Users Section</header>
    <nuxt />
  </div>
</template>

<style>
</style>

<script>
import Header from "@/components/Header";
export default {
  components: {
    Header,
  },
};
</script>