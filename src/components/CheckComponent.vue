<template>
  <div>
    <div>
      <div v-for="(productItem,productIndex) in tranferData" :key = "productIndex">
        <p v-if="productItem.isChecked">Da xac nhan</p>
        <p v-else>Chua xac nhan</p>
      </div>
    </div>
  </div>
</template>

<script>
console.log("I'm CheckComponent");
export default {
  props: [
    'tranferData'
  ],
}
</script>
<style>

</style>