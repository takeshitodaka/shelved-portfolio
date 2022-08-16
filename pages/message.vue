<template>
  <div>
    <form action="send">
      <label for="name">Name</label><br>
      <input id="name" type="text" placeholder="Please input your name"><br>
      <label for="email">E-mail</label><br>
      <input id="email" type="email" placeholder="Please input your mail address"><br>
      <label for="message">Message</label><br>
      <textarea id="message" placeholder="Please input your message" /><br>
    </form>
    <button @click="send">
      send message!
    </button>
  </div>
</template>

<script>

// slackのwebhookメッセージ送信用

const axios = require('axios')
export default {
  name: 'IndexPage',
  methods: {
    send () {
      const params = new URLSearchParams()
      const message = 'Name :\t' + document.getElementById('name').value + '\n Email :\t' + document.getElementById('email').value + '\n Message :\t' + document.getElementById('message').value
      const request = { text: '<!here> \n' + message }
      params.append('payload', JSON.stringify(request))
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
