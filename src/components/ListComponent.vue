<template>
  <div>
    <ItemComponent :tranferData="products"></ItemComponent>
    <CheckComponent :tranferData="products"></CheckComponent>
  </div>
</template>
<script>
import ItemComponent from './ItemComponent.vue'
import CheckComponent from './CheckComponent.vue';
export default {
  components:{
    ItemComponent,
    CheckComponent
  },
  data() {
    return {
      products: [
        {
          id: 1,
          name: 'PS5',
          isChecked: false
        },
        {
          id: 2,
          name: 'PS4',
          isChecked: false
        },
        {
          id: 3,
          name: 'PS3',
          isChecked: false
        }
      ],
      checkId: null
    }
  },

}
</script>
<style>

</style>