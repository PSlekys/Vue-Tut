<template>
  <div class="header">
    <img
      src="https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png"
      alt="Google"
    />

    <nav>
      <a href="#" v-for="link in links" :key="link">{{ link }}</a>
    </nav>
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      links: ["Home", "About", "Contacts"],
    };
  },
};
</script>

<style scoped>
img {
  height: 40px;
  padding: 5px 0;
}

.header {
  background: #eee;
  display: flex;
  justify-content: space-around;
  align-items: center;
}

a {
  margin-right: 10px;
}

a:last-child {
  margin-right: 0;
}
</style>
