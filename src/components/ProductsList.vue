<template>
  <el-row type="flex">
    <el-col
      :span="12"
      v-for="(o, index) in 2"
      :key="o"
      :offset="index > 0 ? 2 : 0"
    >
      <product />
    </el-col>
  </el-row>
</template>

<style></style>


<script lang="ts">
  import {Component, Vue} from 'vue-property-decorator';
  import Product from '@/components/Product.vue';

  @Component({
    components: {
      Product
    },
  })
  export default class ProductsList extends Vue {
  }
</script>
