<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <div class="counter">
      {{ $store. state. counter}}
    </div>
    <div class="counter-squared">
      {{ $store.state.counter}}
      <sup>2</sup> = 
      {{ $store.getters.counterSquared}}

    </div>
    <div class="buttons">
      <button @click="$store.dispatch('decreaseCounter')">-</button>
      <button @click="$store.dispatch('increaseCounter')">+</button>

    </div>
  </div>
</template>

<style>
body {
  background-color: rgb(184, 111, 111);
}
.counter {
  margin-bottom: 10px;
  font-size: 80px;

}
.buttons button {
  font-size: 40px;
  width: 100px;
  margin: 0 10px;

}

</style>
<script>
  export default {

methods: {
 
}
  }

</script>
