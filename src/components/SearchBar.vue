<template>
  <input class="search-bar" id="search" name="search" type="text" placeholder="Search">
</template>



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

/*Futile attemps at vertically centering the placeholder text */
.search-bar{
  height: 40px;
  border-radius: 12px;
  padding: 8px;
  background-image: url('@/assets/search.svg');
    background-size:32px;
    background-position-x: 8px;
    background-position-y:center;
    background-repeat: no-repeat;
    text-indent: 40px;
    border: none;
    color: #1E1E1E;
    line-height: 40px;
    vertical-align: middle;
}

::placeholder{
  color:black;
  font-family: 'Poppins';
  font-weight: 400;
  font-size: 20px;
  line-height: 40px;
  vertical-align: middle;
}
::-webkit-input-placeholder{
  vertical-align: middle;
}

</style>
