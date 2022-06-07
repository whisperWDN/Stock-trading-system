<template>
  <div>
  <el-table
    :data="tableData"
    stripe
    style="width: 100%">
    <el-table-column
      prop="date"
      label="日期"
      width="180">
    </el-table-column>
    <el-table-column
      prop="name"
      label="账户"
      width="180">
    </el-table-column>
    <el-table-column
      prop="type"
      label="申请类型"
      width="180">
    </el-table-column>

    <el-table-column
      label="操作"
      >
      <el-button @click="drawer = true" type="primary" size="small">查看</el-button>
    </el-table-column>
  </el-table>
  <el-drawer

    title="详情"
    v-model="drawer"
    :direction="direction"
    destroy-on-close
  >

    <CheckForm />

  </el-drawer>
  </div>
</template>

<script>
import CheckForm from "@/components/CheckForm.vue";

  export default {
    name:'CheckAView',
    data() {
      return {
        tableData: [{
          date: '2022-05-02',
          name: '王小虎',
          type: '销户'
        }, {
          date: '2022-05-04',
          name: '张无忌',
          type: '开户'
        }, {
          date: '2022-05-01',
          name: '萧峰',
          type: '挂失'
        }, {
          date: '2022-05-03',
          name: '段誉',
          type: '存款'
        }],
        drawer: false,
        innerDrawer: false,
      }
    },
    methods: {
      
    },
    components: {
      CheckForm
    },
    mounted(){
      
    }
  }
</script>