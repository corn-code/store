<template>
  <div id="app">

    <el-container>
      <el-header>
        <header-menu />
      </el-header>

      <el-main>
        <router-view />
      </el-main>

    </el-container>

  </div>
</template>

<style lang="scss">
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }

  #nav {
    padding: 30px;
    a {
      font-weight: bold;
      color: #2c3e50;
      &.router-link-exact-active {
        color: #42b983;
      }
    }
  }
</style>

<script lang="ts">
  import {Component, Vue} from 'vue-property-decorator';
  import HeaderMenu from '@/components/HeaderMenu.vue';

  @Component({
    components: {
      HeaderMenu
    },
  })
  export default class Header extends Vue {
  }
</script>
