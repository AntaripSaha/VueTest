<template>
  <div>
    <button v-on:click="update()">Count Plus +</button>
    <button v-on:click="subtraction()">Count Minus -</button>
    <button v-on:click="multiply(50)">Multiply 50</button>

    <button v-on:click="clear()">Clear</button>
    <input type="text" v-model="count" />
    <h2>Result: {{ count }}</h2>
    <br />
    <br />
    <br />
    <input class="input" placeholder="Email" type="text" v-model="email" />
    <br />
    <br />
    <br />
    <input
      class="input"
      placeholder="Password"
      type="password"
      v-model="password"
    />
    <br />
    <br />
    <br />
    <button type="button" v-on:click="getData()">Submit</button>
  </div>
</template>

<script>
export default {
  name: "Home",
  data() {
    return {
      count: 0,
      email: null,
      password: null,
    };
  },
  methods: {
    update() {
      this.count = this.count + 1;
    },
    subtraction() {
      this.count = this.count - 1;
    },
    multiply(data) {
      this.count = this.count * data;
    },
    clear() {
      this.count = 0;
    },

    getData() {
      console.warn("Values: ", this.email, this.password);
    },
  },
};
</script>

<style scoped>
h1 {
  color: rgb(0, 81, 255);
}

h2 {
  color: rgba(255, 81, 0, 0.644);
}

p {
  color: green;
}

button {
  color: rgb(8, 97, 63);
}

.input {
  border: 2px solid skyblue;
}
</style>
