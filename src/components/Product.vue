<template>

  <el-card :body-style="{ padding: '0px' }">
    <img
      src="@/assets/m3.jpg"
      class="image"
    >
    <div style="padding: 14px;">
      <span>Yummy hamburger</span>
      <el-rate v-model="value1"></el-rate>
      <div class="bottom clearfix">
        <el-button type="primary">Buy</el-button>
      </div>
    </div>
  </el-card>

</template>

<style>
  .time {
    font-size: 13px;
    color: #999999;
  }

  .bottom {
    margin-top: 13px;
    line-height: 12px;
  }

  .button {
    padding: 0;
    float: right;
  }

  .image {
    width: 100%;
    display: block;
  }

  .clearfix:before,
  .clearfix:after {
    display: table;
    content: "";
  }

  .clearfix:after {
    clear: both
  }
</style>

<script>
  export default {
    data() {
      return {
        value1: null
      };
    }
  };
</script>
