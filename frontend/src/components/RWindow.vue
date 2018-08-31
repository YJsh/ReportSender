<template>
  <div style="border: #bfcbd9 solid 1px; margin: 10px">
    <div class="title">{{title}}</div>
    <div style="min-height: 20px">
      <r-table></r-table>
    </div>
  </div>
</template>

<script>
  import RTable from "./RTable";
  export default {
    name: "RWindow",
    components: {RTable},
    data() {
      return {
        title: "这是一个Window"
      }
    }
  }
</script>

<style scoped>
  .title {
    display: flex;
    align-items: center;
    padding: 10px 10px 10px;
    background-color: gray;
    font-size: 20px;
    font-weight: bolder;
    letter-spacing: 1px;
    color: white;
  }
</style>
