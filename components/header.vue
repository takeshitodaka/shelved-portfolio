<template>
  <div>
    <header>
      <h1>Welcome to Takeshi's Portfolilo</h1>
      <HeaderNav />
    </header>
  </div>
</template>

<script>
import HeaderNav from '@/components/headerNav.vue'
export default {
  components: {
    HeaderNav
  }
}
</script>
<style scoped>
  @import "~/assets/css/navs.css";
</style>
