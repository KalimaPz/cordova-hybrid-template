<template>
  <div>
      <p>{{ this.$store.state.count }}</p>
      <p><button @click="inc">count+</button></p>
      <p><button @click="dec">count-</button></p>
  </div>
  
</template>

<script>
export default {
    name : "Counter",
    methods: {
        inc() {
            this.$store.state.count++;
        },
         dec() {
            this.$store.state.count--;
        }
    },
}
</script>

<style>

</style>