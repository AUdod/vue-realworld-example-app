<template>
  <footer>
    <div class="container">
      <router-link
        class="logo-font"
        :to="{ name: 'home', params: {} }"
        id="footer-brand"
      >
        FintechSquad's bondage gay website
      </router-link>
      <span class="attribution">
        An interactive learning project from
        <a rel="noopener noreferrer" target="blank" href="https://thinkster.io"
          >Thinkster</a
        >. Code &amp; design licensed under MIT.
      </span>
    </div>
  </footer>
</template>

<script>
export default {
  name: "RwvFooter"
};
</script>

<style>
#footer-brand {
  background-image: linear-gradient(
    to left,
    violet,
    indigo,
    blue,
    green,
    yellow,
    orange,
    red
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
</style>
