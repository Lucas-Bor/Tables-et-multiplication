<template>
  <div>
    <h3>Table de {{n}}</h3>
    <table class="table-multiplication" >
      <tbody>
        <div v-for="k in 10" v-bind:key="k">
         <TableRow v-bind:j="k" v-bind:i="n"/>
        </div>
      </tbody>
    </table>
    <br/>
  </div>
</template>

<script>
  import TableRow from "./TableRow.vue";

  export default {
    name: "TableMultiplication",
    props: {
      n : Number
    },
    components: {
      TableRow
    },
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .table-multiplication {
    text-align: center;
    margin-left: auto;
    margin-right: auto;
    background-color: grey;
  }
</style>
