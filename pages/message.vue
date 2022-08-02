<template>
  <div>
    <button @click="send">
      test
    </button>
  </div>
</template>

<script>
const axios = require('axios')
export default {
  name: 'IndexPage',
  methods: {
    send () {
      const params = new URLSearchParams()
      const message = { text: 'test message' }
      params.append('payload', JSON.stringify(message))
      axios.post(this.$config.SLACK_URL, params).then((res) => {
        console.log(res)
      }).catch((err) => {
        console.log(err)
      })
    }
  }

}
</script>
<style scoped>

</style>
