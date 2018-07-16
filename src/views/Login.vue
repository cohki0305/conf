<template lang="pug">
  div
    button(@click="login")
      | Login
</template>

<script>
import firebase from 'firebase'

export default {
  methods: {
    async login() {
      const provider = new firebase.auth.TwitterAuthProvider()
      try {
        await firebase.auth().signInWithPopup(provider)
      } catch (e) {
        console.log(e)
      }
    }
  }
}
</script>

<style>

</style>
