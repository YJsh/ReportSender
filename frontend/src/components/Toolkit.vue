<template>
  <el-menu>
    <el-menu-item index="RHeadline" @click="test(index)">RHeadline 标题</el-menu-item>
    <el-menu-item index="RTable">RTable 表格</el-menu-item>
  </el-menu>
</template>

<script>
    export default {
        name: "Toolkit",
      methods: {
          test(index) {
            console.log(index)
          }
      }
    }
</script>

<style scoped>

</style>
