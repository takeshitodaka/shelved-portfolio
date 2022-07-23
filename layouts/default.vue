<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div>
    <main>
      <Header />
      <nuxt />
    </main>
    <Footer />
  </div>
</template>
<script>
import Header from '@/components/header.vue'
import Footer from '@/components/footer.vue'
export default {
  components: {
    Header,
    Footer
  }

}
</script>
<style scopped>
    main {
        min-height: 600px;
        background-color: rgb(203, 199, 255);
        text-align: center;
        padding: 30px;
    }
        .page-enter-active,
    .page-leave-active {
        transition: 0.5s cubic-bezier(1, 0.25, 0.25, 1);
    }
    .page-enter,
    .page-leave-active {
        opacity: 0;
        transform: translate(0, 30px);
    }
</style>
