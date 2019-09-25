<template>
  <div>
    <section class="section-scroll">
      <navigation-bar></navigation-bar>
      <Header></Header>
      <Footer></Footer>
    </section>
  </div>
</template>
<script>
import Header from "./components/Header.vue";
import NavigationBar from "./components/NavigationBar.vue";
import Footer from "./components/Footer.vue";
export default {
  components: {
    Header: Header,
    NavigationBar: NavigationBar,
    Footer: Footer
  }
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  font-family: "Poppins", sans-serif;
  scroll-behavior: smooth;
}
</style>
