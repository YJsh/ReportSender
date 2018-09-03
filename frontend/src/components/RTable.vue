<template>
  <el-table :data="tableData" border :show-header="false">
    <el-table-column v-for="(col, index) in colNum" :key="col" label="">
      <template slot-scope="scope">
        {{scope.row[index]}}
      </template>
    </el-table-column>
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
