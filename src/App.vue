<template>
    <the-header />
    <the-main />
    <the-footer />
</template>

<script>

import TheHeader from "@/components/TheHeader";
import TheFooter from "@/components/TheFooter";
import TheMain from "@/components/TheMain";


export default {
  name: 'App',
  components: {
      'the-header': TheHeader,
      'the-footer': TheFooter,
      'the-main': TheMain,
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@100;200;300;400;500;600;700;800;900&display=swap');

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
    text-decoration: none;
    list-style: none;
}

.container {
    margin: 0 auto;
    max-width: 1240px;
}
</style>
