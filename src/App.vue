<script>
import { defineSSRCustomElement } from 'vue';
import Count from './components/Count.vue';
import Counter from './components/Counter.vue';

export default {

  data() {
    return {
      count: 0
    }
  },

  components: {
    Count,
    Counter
  },


  methods: {
    increment() {
      this.count = this.count + 1

    },

    decrement() {
      this.count = this.count - 1
    }

  }
}


</script>

<template>
  <main>
    <div class="container">
      <div class="row">
        <h1 class="text-center mb-5">Contatore</h1>
        <Counter :counter="count"></Counter>
        <Count @increment="increment()" @decrement="decrement()"></Count>
      </div>
    </div>

  </main>
</template>


<style>
main {
  background-color: #ed5b27;
  color: white;
  height: 100vh;
}
</style>