<template>
    <el-descriptions title="申请信息" column="1">
        <el-descriptions-item label="账号">A65659</el-descriptions-item>
        <el-descriptions-item label="姓名">张无忌</el-descriptions-item>
        <el-descriptions-item label="联系方式">18888888888</el-descriptions-item>
        <el-descriptions-item label="申请类型">开户</el-descriptions-item>
        <el-descriptions-item >
            <el-button type="primary" @click="onSubmit">通过</el-button>
            <el-button type="primary" @click="onSubmit">拒绝</el-button>
        </el-descriptions-item>

    </el-descriptions>
</template>

<script>
  export default {
    name:'CheckForm',
    data() {
      return {

      }
    },
    props:[
        
    ],
    methods: {

    }
  }
</script>