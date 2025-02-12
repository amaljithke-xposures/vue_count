<template>
  <div id="app">
    <!-- Navigation links -->
    <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>

  <H1>COUNT THE NUMBER</H1>
    </nav>

    <!-- Render the views based on the route -->
    <router-view />
  </div>
</template>

<script setup>
// No additional script setup needed here
</script>

<style scoped>
/* Basic styles for navigation */
nav {
  margin: 20px;
  font-size: 20px;
}

router-link {
  margin: 0 10px;
  text-decoration: none;
  color: #333;
}

router-link:hover {
  color: #007BFF;
}

#app{
text-align: center;
}
</style>
