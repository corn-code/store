<template>
  <div class="home">

    <products-list />

    <subscription-form />

  </div>
</template>

<script lang="ts">
  import {Component, Vue} from 'vue-property-decorator';
  import ProductsList from '@/components/ProductsList.vue';
  import SubscriptionForm from '@/components/SubscriptionForm.vue';

  @Component({
    components: {
      ProductsList,
      SubscriptionForm
    },
  })
  export default class Home extends Vue {
  }
</script>
