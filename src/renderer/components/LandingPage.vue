<template>
  <div id="landing-page">
    <h1>Hello World!</h1>
    <button @click="open('https://github.com/tobyryuk/electron-vue-base/')">Start</button>
  </div>
</template>

<script>
export default {
  name: 'landing-page',
  methods: {
    open (link) {
      this.$electron.shell.openExternal(link)
    }
  }
}
</script>
