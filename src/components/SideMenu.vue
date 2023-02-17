
<template>
  <section class="menu">
  <div class="dashboard-div">
    <img src="@/assets/vectorA.svg" alt="">
    <p class="dash-p">Dashboard</p>
  </div>
  <ul>
    <li>
      <!--<MenuLink imgName="src/assets/invoice.svg" title="Invoices"  />-->
      <div>
        <img class="menu-img" src="@/assets/invoice.svg" alt=""/>
        <p>Invoices</p>
      </div>
    </li>
    <li>
      <div>
        <img class="menu-img" src="@/assets/people.svg" alt="">
        <p>Clients</p>
      </div>
    </li>
    <li>
      <div>
        <img class="menu-img" src="@/assets/box.svg" alt="">
        <p>Products</p>
      </div>
    </li>
    <li>
      <div>
        <img class="menu-img" src="@/assets/enveloppe.svg" alt="">
        <p>Messages</p>
      </div>
    </li>
    <li>
      <div>
        <img class="menu-img" src="@/assets/settings.svg" alt="">
        <p>Settings</p>
      </div>
    </li>
    <li>
      <div>
        <img class="menu-img" src="@/assets/question.svg" alt="">
        <p>Help</p>
      </div>
    </li>
  </ul>
  <div>
    <img src="@/assets/logout.svg" alt="">
    <p>Logout</p>
  </div>
</section>
<ul class="icon-bar">
  <li>
    <img src="@/assets/vectorA.png">
  </li>
  <li>
    <img src="@/assets/invoice.svg">
  </li>
  <li>
    <img src="@/assets/people.svg">
  </li>
  <li>
    <img src="@/assets/box.svg">
  </li>
  <li>
    <img src="@/assets/enveloppe.svg">
  </li>
  <li>
    <img src="@/assets/settings.svg">
  </li>
  <li>
    <img src="@/assets/question.svg">
  </li>
  <li>
    <img src="@/assets/logout.svg">
  </li>
</ul>
</template>

<script>
//import MenuLink from "./MenuLink.vue"
export default {
  name: 'SideMenu',
  /*components: {
    MenuLink
  }*/
}
</script>

<style scoped>
.icon-bar{
  display: none;
}
div{
  display: flex;
  align-items: center;
  gap:17px;
}
.menu-img{
  width:48px;
}
.menu{
  margin-left: 16px;
}
div{
  margin-left: 32px;
}
ul{
  list-style: none;
}
li{
  margin-bottom:32px;
}
p{
  color: rgba(255,255,255,0.8);
  opacity: 0.8;
}
.dash-p{
  color:#1E1E1E;
  opacity: 1;
  font-weight: 400;
  font-size: 25px;
  line-height: 38px;

}
.dashboard-div{
  background-image: linear-gradient(266.37deg, #FAFF00 -5.82%, #FAFF00 15.95%, #1970D6 41.2%, #6C1182 72.88%);
  border-radius: 17px;
  height: 65px;
  display: flex;
  align-items: center;
  justify-content: center;
  gap:17px;
  padding: 16px;
  margin-left: 0;
  margin-bottom: 16px;

}
/*section{
  position: absolute;
  top: 0;
}*/
.burger{
  display: none;
}
@media(max-width: 900px){
.menu{
  display: none;
  position:fixed;
  top: 130px;
}
.icon-bar{
  display: flex;
  flex-direction: column;
  position: absolute;
  top: 130px;
  left:8px;
}
img{
  width:32px;
}
}
</style>