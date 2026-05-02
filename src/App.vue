<template>
  <h1>Hi {{ firstName.toUpperCase() }} !</h1>
  <p>You are the GOAT.</p>
</template>

<script setup>
  const firstName = "Leo";
</script>

<style>
h1 {
  color: pink;
}
p {
  font-size: 4ch;
}
</style>