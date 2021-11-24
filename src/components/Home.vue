<template>
  <div>
    <button v-on:click="update()">Count Plus +</button>
    <button v-on:click="subtraction()">Count Minus -</button>
    <button v-on:click="multiply(50)">Multiply 50</button>
    <button v-on:click="click()">Clear</button>
    <input type="text" v-model="count" />
    <h2>{{ count }}</h2>
    <h1>Email: {{ email }}</h1>
    <P> Mobile: {{ mob }}</P>
    <P> Name: {{ getData("Dip Saha") }}</P>
    <P> Name: {{ getInfo().Name }}</P>
    <P> Email: {{ getInfo().Email }}</P>
    <P> Function: {{ math(50) }}</P>
  </div>
</template>

<script>
export default {
  name: "Home",
  data() {
    return {
      email: "antarip15@gmail.com",
      mob: "00200202",
      count: 0,

      math: function (a) {
        return 10 * a;
      },
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
    getData(name) {
      return name;
    },
    getInfo() {
      return {
        Name: "Antarip Saha",
        Email: this.email,
      };
    },

    click() {
      this.count = 0;
    },
  },
};
</script>

<style scoped>
h1 {
  color: rgb(0, 81, 255);
}
h2 {
  color: rgb(0, 255, 13);
}

p {
  color: green;
}

button {
  color: rgb(8, 97, 63);
}
</style>
