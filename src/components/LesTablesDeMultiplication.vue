<template>
  <div>
    <div class="table" v-for="m in 13" v-bind:key="m" >
      <h3>Table de {{m}}</h3>
      <table class="table-de-multiplication">
        <tbody>
          <div v-for="k in 10" v-bind:key="k">
            <TableRow v-bind:j="k" v-bind:i="m"/>
          </div>
        </tbody>
      </table>
    </div>
  </div>
</template>

<script>
  import TableRow from "./TableRow.vue";

  export default {
    name: "TableDeMultiplication",
    props: {
      n : Number
    },
    components: {
      TableRow
    },
  }
</script>
<style scoped>
  .table{
    display: inline-block;
    margin-left: 20px;
  }
  .table-de-multiplication{
    background-color: grey;
  }
</style>