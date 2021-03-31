<template>
  <div id="app" :style="{ backgroundColor: `RGB(${red},${green},${blue})` }">
    <p>Поля ввода компонентов RGB и бегунки:</p>
    <p>
      R:
      <input v-model="red" type="number" min="0" max="255" value="255" /><input
        type="range"
        min="0"
        max="255"
        v-model="red"
      />
    </p>
    <p>
      G:
      <input
        v-model="green"
        type="number"
        min="0"
        max="255"
        value="255"
      /><input type="range" min="0" max="255" v-model="green" />
    </p>
    <p>
      B:
      <input v-model="blue" type="number" min="0" max="255" value="255" /><input
        type="range"
        min="0"
        max="255"
        v-model="blue"
      />
    </p>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      red: 255,
      green: 255,
      blue: 255,
    };
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  height: 100%;
}
p {
  font-size: 20px;
  font-weight: bold;
}
</style>
