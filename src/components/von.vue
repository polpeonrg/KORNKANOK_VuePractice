<template>
  <div>
    <h1>V-On</h1>
    <h2>{{ message }}</h2>
    <button v-on:click="add()">Add</button>
    <!-- 
      <button v-on:click="message = message - 1">Del</button>
    -->
  </div>
</template>

<script>
export default {
  data() {
    return {
      message: 0,
    };
  },
  methods: {
    add() {
      this.message = this.message + 1;
    },
  },
};
</script>