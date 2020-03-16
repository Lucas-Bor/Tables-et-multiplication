<template>
  <div>
    <br>
    <label for="user-input2"> Entrez une valeur : </label>
    <input id="user-input-2" type="text" v-model="v">
    <label for="user-input3"> Et une deuxième : </label>
    <input id="user-input-3" type="text" v-model="m">
    <p>
      <small style="font-style:italic;">(Les valeurs entrée sont {{v}} et {{m}})</small>
    </p>
    <MultiplicationUnique v-bind:v="parseInt(v)" :m="parseInt(m)"/>
    <hr/>
  </div>
</template>

<script>
  import MultiplicationUnique from "./MultiplicationUnique.vue";
  export default {
    name: "TaMultiplication",
    data: function () {
      return {
        v : 1,
        m : 2
      };
    },
    components: {
      MultiplicationUnique,
    }
  };
</script>

<style>
  #app {
    font-family: "Avenir", Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;

    margin-top: 60px;
  }

</style>