<template>
  <h1>A single user, with ID: {{ $route.params.id }}</h1>
</template>

<script>
export default {
  validate(data) {
    console.log(data);
    // validating if the input value is a number. If so it lets you go on.
    return /^\d+$/.test(data.params.id);
  },
  layout: "users",
};
</script>