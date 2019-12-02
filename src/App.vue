<template>
  <div>
    <h1>Clicked {{ count }} times.</h1>
    <button @click="Increment()">Click me!</button>
    <button @click="Reset">Click to reset.</button>
  </div>
</template>

<script>
  export default {
    data() {
      return {title: 'Not clicked yet',
      count: 0
      }
    },
    methods: {
      Increment() {
        this.title = 'Clicked';
        this.count = this.count+1;
      },
      Reset() {
        this.count = 0;
      }
    }
  };
</script>

