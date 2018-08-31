<template>
  <el-table :data="tableData" border size="mini">
    <el-table-column v-for="col in colNum" :key="col" label=""></el-table-column>
  </el-table>
</template>

<script>
  export default {
    name: "RTable",
    data() {
      return {
        colNum: 3,
        rowNum: 3,
      }
    },
    computed: {
      tableData() {
        let data = [];
        for (let row = 0; row < this.rowNum; row++) {
          data.push(Array(this.colNum).fill(""));
        }
        return data;
      }
    }
  }
</script>

<style scoped>

</style>
