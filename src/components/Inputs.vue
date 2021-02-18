<template>
  <div>
    <label>Value 1 :</label>
    <input
      type="number"
      placeholder="Enter the value"
      v-model="value1"
      required
    />
    <label>Value 2 :</label>
    <input
      type="number"
      placeholder="Enter the value"
      v-model="value2"
      required
    />
    <label>Sum :</label>
    <h1>{{ sum(value1, value2) }}</h1>
  </div>
</template>

<script>
export default {
  name: "Inputs",
  data() {
    return {
      value1: 0,
      value2: 0,
    };
  },
  methods: {
    sum: function (value1, value2) {
      if (value1 !== "" && value2 !== "") {
        return parseInt(value1) + parseInt(value2);
      } else {
        return "Please put value in the empty input";
      }
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
div {
  display: flex;
  flex-direction: column;
  margin: 0 auto;
  padding: 2rem;
  max-width: 600px;
}

input {
  padding: 1rem;
  margin: 1rem 0;
  border-radius: 10px;
}
</style>
