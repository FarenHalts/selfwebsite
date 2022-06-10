<template>
  <div class="home">
    <input type="number" v-model="inputData">
    <div v-if="inputData">{{squareRoot}}</div>
  </div>
</template>

<script>

export default {
  name: 'HomeView',
  data(){
    return{
      inputData: ''
    }
  },
  computed: {
    squareRoot(){
      return Math.sqrt(this.inputData)
    }
  }
}
</script>
