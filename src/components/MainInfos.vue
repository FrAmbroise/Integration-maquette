<template>
  <div class="main-infos">
    <div class="flex-row">
      <div class="wallet-summary">
      <h2>Total balance</h2>
      <div class="btc-number">
        <p class="big-number">0.874995497</p>
        <img src="@/assets/Btc.png" class="btc-img" alt="">
      </div>
      <p class="moni">$42,874.98</p>
    </div>
    <div class="portfolio">
      <p class="bg-black">Portfolio</p>
      <p>Funding</p>
      <p>Assets</p>
      <p>P2P</p>
    </div>
  
  </div>


    <img src="@/assets/The_Graph_TM.png" alt="">
    <div class="see-coin">
      <p>Recent transactions</p>
      <p class="grey-p">See all coins</p>
    </div>

    <div class="recent-transactions">
      <div class="bitcoin">
        <img class="icon" src="@/assets/bitcoin.svg" alt="">
        <div class="flex-col">
          <p class="op9 name">Bitcoin</p>
          <p class="abreviation grey-p">BTC</p>
        </div>
        <div class="flex-col">
          <p class="market-p op9">Market cap</p>
          <p class="market-rate blue grey-p">$40,001.63</p>
        </div>
        <div class="flex-col">
          <p class="h-p op9">24h change</p>
          <p class="h-value red grey-p">-2.02</p>
        </div>
        <div class="squiggle">
          <img src="@/assets/purple_wave.svg">
        </div>
        <button>Trade</button>
      </div>
      <div class="bitcoin">
        <img class="icon" src="@/assets/Etherum_icon.svg" alt="">
        <div class="flex-col">
          <p class="name op9">Etherum</p>
          <p class="abreviation grey-p">ETH</p>
        </div>
        <div class="flex-col">
          <p class="market-p op9">Market cap</p>
          <p class="market-rate purple grey-p">$39,735.03</p>
        </div>
        <div class="flex-col">
          <p class="24-p op9">24h change</p>
          <p class="24-value green grey-p">+6.12</p>
        </div>
        <div class="squiggle">
          <img src="@/assets/blue_wave.svg">
        </div>
        <button>Trade</button>
      </div>
    </div>
  </div>




</template>

<script>
export default {
  name:'MainInfos'

}
</script>

<style scoped>
h2{
  font-family: 'Poppins';
font-style: normal;
font-weight: 900;
font-size: 22px;
line-height: normal;
opacity: 0.8;
color:white;
margin:  8px 0 8px 0;
}
.flex-row{
  display: flex;
  gap: 60px;
}

.see-coin{
  font-family: 'Poppins';
font-style: normal;
font-weight: 700;
font-size: 22px;
display: flex;
color: white;
justify-content: space-between;
padding-left: 25px;

}
.bg-black{
  background-color: #000;
  border-radius: 8px;
  padding: 4px;
}
.portfolio{
  display: flex;
  flex-wrap: wrap;
  justify-content: space-evenly;
  align-items: center;
  color: white;
  background: #292727;
border-radius: 16px;
padding: 16px;
width: 60%;
gap:16px;
}
.recent-transaction p{
  font-family: 'Inter';
}

.big-number{
  font-family: 'Poppins';
font-style: normal;
font-weight: 700;
font-size: 29px;
color:white;
line-height: normal;
margin:  8px 0 8px 0;
}
.btc-img{
  height: 25px;
}
.btc-number{
  display: flex;
  justify-content: center;
  align-items: center;
  gap:16px;
  line-height: normal;
  margin: 8px 0 8px 0;
}
.moni{
  font-family: 'Poppins';
  font-style: normal;
  font-weight: 600;
  font-size: 22px;
  opacity:0.7;
  color:white;
  line-height: normal;
  margin:  8px 0 8px 0;
}
.blue{
  color: #1970D6;
  opacity: 0.7;
}
.purple{
  color:#6C1182;
  opacity: 0.7;
}
.wallet-summary{
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}
/*.main-infos{
  margin-left: 360px;
  top:0px;
}*/
.top-main{
  display: flex;
  align-items: center;
}
h1{
  color: white;
  font-family: 'Poppins';
  font-weight: 500;
  font-size: 35px;
}
.search-bar{
  border-radius: 16px;
  height: 40px;
  width: 200px;
}
img{
  text-align: unset;
  max-width: 95%;
}
.icon{
  height: 32px;
}
.bitcoin{
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-evenly;
  color:white;
  background: rgba(32, 35, 43, 0.7);
  border-radius: 8px;
  margin-bottom:16px;
}
.bitcoin p{
  font-family: 'Inter';
}
.op9{
  opacity: 0.95;
}
.grey-p{
  opacity: 0.7;
}
.flex-col{
  display: flex;
  flex-direction: column;
}

button{
  background-color: #000;
  color: white;
  border-radius: 16px;
  border:none;
  padding: 8px;
}
@media(max-width: 1200px){
  .portfolio{
    display: grid;
    grid-template-columns: repeat(2, 1fr);
  }
}
@media(max-width: 900px){
  .main-infos{
    margin-left: 40px;
    margin-right: 16px;
  }
}

@media(max-width: 768px){
  .see-coin{
    flex-direction: column;
  }
  .squiggle{
    display: none;
  }
  .portfolio{
    display: flex;
  }
  .flex-row{
    flex-direction: column;
    gap:24px;
    margin-bottom: 40px;
  }
}
@media(max-width: 600px){
  .portfolio{
    display: grid;
    width: auto;
    grid-template-columns: repeat(2, 1fr);
  }
}
@media(max-width: 500px){
  .bitcoin{
    flex-direction: column;
  }
}
</style>