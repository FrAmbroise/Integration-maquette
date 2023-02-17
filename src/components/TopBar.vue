<template>
  <div class="top-bar">
    <div class="logo-div">
      <img class="grologo" src="../assets/minance.svg" alt="">
      <img class="pitilogo" src="@/assets/m_logo.svg" alt="">
    </div>
    <div class="top-main">
      <h1>Hi, Rogers</h1>
      <SearchBar class="search-bar"/>
    </div>
    <div class="top-account">
      <img class="bell" src="@/assets/bell.svg">
      <img src="@/assets/user_icon.png">
    </div>
  </div>

</template>

<style>
.top-bar{
  display: grid;
  grid-template-columns: 0.8fr 2fr 0.7fr;
  margin: 8px;

}
.logo-div{
  grid-column: 1/2;
  grid-row: 1/2;
  display: flex;
  align-items: center;
}
.pitilogo{
  display:none;
}
.top-main{
  grid-column: 2/3;
  grid-row: 1/2;
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: white;
}
.top-account{
  grid-column: 3/4;
  grid-row: 1/2;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 32px;

}
h1{
  font-weight: 500;
  font-style: normal;
}
@media(min-width: 1024px){
  .search-bar{
    width: 360px;
  }
}
@media(max-width: 768px){
  .grologo{
    display: none;
  }
  .pitilogo{
    display: block;
  }
  h1{
    display:none;
  }
  .top-main{
    justify-content: center;
  }
  .top-account{
    padding:8px;
  }

}
@media (max-width:500px){
  .search-bar{
    width:150px;
  }
}
@media(max-width: 425px){
  .bell{
    display: none;
  }
}
</style>
<script>
import SearchBar from "./SearchBar.vue"
export default {
  name:'TopBar',
  components: {
    SearchBar
  }

}

</script>
