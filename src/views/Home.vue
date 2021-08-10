<template>
  <div class="Index">
    <shortcut></shortcut>
    <Header></Header>
    <main-body />
    <main-body-content />
    <Footer class="footer-1" />
  </div>
</template>

<script>
import Shortcut from "components/common/Shortcut";
import Header from "components/common/Header";
import MainBody from "components/content/MainBody";
import MainBodyContent from "components/content/MainBodyContent";
import Footer from "components/common/Footer";
export default {
  name: "Home",
  components: {
    Shortcut,
    Header,
    MainBody,
    MainBodyContent,
    Footer,
  },
};
</script>
<style>
</style>