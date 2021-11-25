<template>
<div>
    <h1>Check Box Get Data</h1>

    <h3>Technology</h3>
    <label for="java">Java</label>
    <input type="checkbox" value="java" v-model="technology" id="java" />
    <br />
    <label for="php">Php</label>
    <input type="checkbox" value="php" v-model="technology" id="php" />
    <br />
    <label for="node">Node</label>
    <input type="checkbox" value="node" v-model="technology" id="node" />

    <br />
    <h4>Technology: {{ technology }}</h4>

    <br />
    <br />
    <h3>Who Am I</h3>
    <label for="developer">Developer</label>
    <input type="radio" id="developer" name="des" value="developer" v-model="designation" />

    <label for="student">Student</label>
    <input type="radio" id="student" name="des" value="student" v-model="designation" />

    <h4>I Am A: {{ designation }}</h4>
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
</div>
</template>

<script>
export default {
    name: "CheckBox",
    data() {
        return {
            technology:[],
            designation: null,
        };
    },
};
</script>

<style scoped>
h4 {
    color: rgb(47, 144, 151);
}
</style>
