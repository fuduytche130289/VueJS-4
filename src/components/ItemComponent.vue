<template>
  <div>
    <div>
      <div v-for="(productItem,productIndex) in tranferData" :key = "productIndex">
        {{ productItem.name }}
      </div>
    </div>
  </div>
</template>

<script>
console.log("I'm ItemComponent");
export default {
  props: [
    'tranferData'
  ],
}
</script>
<style>

</style>