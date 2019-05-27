<template>
  <div style="margin: 20px;">
    <el-date-picker v-model="value1" type="date" :picker-options="pickerOptions1" />
    <el-divider></el-divider>
    <el-date-picker v-model="value2" type="week" format="yyyy-MM-dd" value-format="yyyyMMdd" :picker-options="pickerOptions1" />
    <el-divider></el-divider>
    <el-date-picker v-model="value3" type="month" :picker-options="pickerOptions1" />
    <el-divider></el-divider>
    <el-date-picker v-model="value4" type="daterange" :picker-options="pickerOptions2" />
    <el-divider></el-divider>
    <el-date-picker v-model="value5" type="weekrange" :picker-options="pickerOptions2" />
    <el-divider></el-divider>
    <el-date-picker v-model="value6" type="monthrange" :picker-options="pickerOptions2" />
    <el-divider></el-divider>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        value1: '',
        value2: '',
        value3: '',
        value4: '',
        value5: '',
        value6: '',
        pickerOptions1: {
          firstDayOfWeek: 1,
          showConfirmButton: false
        },
        pickerOptions2: {
          firstDayOfWeek: 1,
          showConfirmButton: true
        }
      };
    }
  };
</script>
