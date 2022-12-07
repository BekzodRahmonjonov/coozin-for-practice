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
.container {
    margin: 0 auto;
    max-width: 1240px;
}
</style>
