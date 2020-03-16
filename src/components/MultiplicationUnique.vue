<template>
  <div>
    <h3>Ta multiplication</h3>
    <table class="table-multiplication" >
         <TableRow v-bind:j="m" v-bind:i="v"/>
    </table>
  </div>
</template>

<script>
  import TableRow from "./TableRow.vue";

  export default {
    name: "MultiplicationUnique",
    props: {
      v : Number,
      m : Number
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
