<template>

  <div>
    <img :src="iconpath" alt="">
    <div class="flex-col">
      <p>{{ name }}</p>
      <p>{{ status }}</p>

    </div>
    <div class="flex-col">
      <p>{{ amount }}</p>
      <p>{{ date }}</p>
    </div >
  </div>
</template>

<script>
export default {
  name:"BasicTransaction",
  props:['name','status','amount', 'date','iconPath']
}

</script>
<style>
.flex-col{
  display: flex;
  flex-direction: column;
}
</style>