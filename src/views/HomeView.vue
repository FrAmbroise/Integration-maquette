<template>
  <div class="home">
    <TopBar class="the-top"/>
    <main>
      <MainInfos class="main-info"/>
      <SideMenu class="side-menu"/>
      <RightInfos class="right-info"/>
      <!--canvas id="myChart"></canvas-->
    </main>

  </div>
</template>

<script>
// @ is an alias to /src
import SideMenu from '@/components/SideMenu.vue'
import MainInfos from '@/components/MainInfos.vue'
import RightInfos from '@/components/RightInfos.vue'
import TopBar from '@/components/TopBar.vue'
//import Chart from 'chart.js'

export default {
  name: 'HomeView',
  /*mounted() {
    const ctx = document.getElementById('myChart').getContext('2d')
    new Chart(ctx, {
      type: 'line',
      data: {
        labels: ['5Nov', '6Nov', '7Nov','8Nov','9Nov', '10Nov', '11Nov', '12Nov', '13Nov', '14Nov', '15Nov'],
        datasets: [
          {
            label: 'ETH',
            data: [100, 400,600, 400, 300, 100, 350, 200, 300, 700, 600]
          }
        ]
      }
    })
  },*/
  components: {
    SideMenu,
    MainInfos,
    RightInfos,
    TopBar
  },
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Poppins';
}
.transaction p{
  font-family: 'Inter';
}
body{
  background-color: #1E1E1E;

}
main{
  display: grid;
  grid-template-columns: 8fr 20fr 12fr;
  grid-gap: 16px;
  max-width: 100%;
}
.side-menu{
  grid-column: 1/2;
  grid-row:1/2;
}
.main-info{
  grid-column: 2/3;
  grid-row:1/2;
  max-width: 100%;
}
.right-info{
  grid-column: 3/4;
  grid-row:1/2;
}
@media(max-width:900px){
  main{
    grid-template-columns: 19fr 10fr;
  }
  .main-info{
    grid-column: 1/2;
    padding-left:32px;
  }
  .right-info{
    grid-column: 2/3;
  }
}
@media (max-width: 768px){
  main{
    display: block;
  }


}
</style>
