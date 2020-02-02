<template>
  <div>
    aaa
  </div>
</template>

<script>
export default {
  // components: {
  // }
  data() {
    return {
      player: 2,
      turn: 15
    }
  },
  created: {},
  methods: {
    random_sort(array) {
      for(let i = array.length - 1; i > 0; i--) {
        let r = Math.floor(Math.random() * (i + 1))
        let tmp = array[i]
        array[i] = array[r]
        array[r] = tmp;
      }
    }
  }
}
</script>

<style scoped></style>
