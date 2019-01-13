<template>
  <el-row>

    <el-col :span="12" :offset="6">
      <el-form
        :inline="true"
        :model="formInline"
        class="demo-form-inline"
      >
        <el-form-item>
          <el-input
            v-model="formInline.user"
            placeholder="my@email.com"
          ></el-input>
        </el-form-item>
        <el-form-item>
          <el-button
            type="primary"
            @click="onSubmit"
          >Subscribe
          </el-button>
        </el-form-item>
      </el-form>
    </el-col>

  </el-row>
</template>

<style>
  .el-row {
    margin-bottom: 20px;
    &:last-child {
       margin-bottom: 0;
    }
  }
</style>

<script>
  export default {
    data() {
      return {
        formInline: {
          user: "",
          region: ""
        }
      };
    },
    methods: {
      onSubmit() {
        console.log("submit!");
      }
    }
  };
</script>

