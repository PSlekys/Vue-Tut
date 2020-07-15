<template>
  <div id="app">
    <Header />
    <ToDo />
  </div>
</template>

<script>
import Header from "./components/Header";
import ToDo from "./components/ToDo";

export default {
  name: "App",
  components: { Header, ToDo },
};
</script>
