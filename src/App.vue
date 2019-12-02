<template>
  <div>
    <h1>{{ text }}</h1>
    <button @click="ChangeMood()">Click to change.</button>
  </div>
</template>

<script>
  export default {
    data() {
      return {happy: false,
        text: 'Sad :('
      }
    },
    methods: {
      Increment() {
        this.title = 'Clicked';
        this.count = this.count+1;
      },
      Reset() {
        this.count = 0;
      },
      ChangeMood() {
        this.happy=!this.happy;
        this.text=this.happy ? 'Happy :)' : 'Sad :(';
      }
    }
  };
</script>

