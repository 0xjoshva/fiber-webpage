<template>
  <TheNavbar/>
  <router-view/>
  <TheFooter/>
</template>
<script>
import TheNavbar from '@/components/TheNavbar.vue';
import TheFooter from '@/components/TheFooter.vue';

export default {
  components: {
    TheNavbar, TheFooter
  }
}
</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;700;800;900&display=swap');
/* font-family: 'Inter', sans-serif */

*, *::before, *::after {
  box-sizing: border-box;
}
* {
  margin: 0;
}
html, body {
  height: 100%;
  font-family: 'Inter', sans-serif
}
body {
  line-height: 1.5;
  -webkit-font-smoothing: antialiased;
}
img, picture, video, canvas, svg {
  display: block;
  max-width: 100%;
}
input, button, textarea, select {
  font: inherit;
}
p, h1, h2, h3, h4, h5, h6 {
  overflow-wrap: break-word;
}
#root, #__next {
  isolation: isolate;
}

:root{
  --black:black;
  --text: #4F4F4F;
  --blue: #4D13D1;
  --white: #ffffff;
  --lgrey: #DEDEDE;
}
</style>


