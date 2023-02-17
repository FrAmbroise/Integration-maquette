<template>

  <img :src="imgName" alt=""/>
  <p>{{ title }}</p>
</template>

<script>
export default {
  name:"MenuLink",
  props:['imgName','title']
}
</script>

<style scoped>
p{
  color:rgba(255, 255, 255, 0.8);
  opacity: 0.8;
  font-family: 'Poppins';
}
</style>