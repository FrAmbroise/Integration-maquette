<template>
  <div class="right-info">
    <div>
      <p class="right-title">Recent Transactions</p>
    </div>
    <div class="transaction">
      <img src="@/assets/t_icon.svg" alt="">
      <div class="flex-col">
        <p>Usdt</p>
        <p class="grey">Received</p>
      </div>
      <div class="flex-col">
        <p class="green">+$3,754</p>
        <p class="grey">Today 7:24pm</p>
      </div>
    </div>
    <div class="transaction">
      <img src="@/assets/bnb_icon.svg" alt="">
      <div class="flex-col">
        <p>BNB</p>
        <p class="grey">Buy</p>
      </div>
      <div class="flex-col">
        <p class="green">+$0.5460</p>
        <p class="grey">Today 3:01pm</p>
      </div>
    </div>
      <div class="transaction">
      <img src="@/assets/L_icon.svg" alt="">
      <div class="flex-col">
        <p>Lite coin</p>
        <p class="grey">Withdrawal</p>
      </div>
      <div class="flex-col">
        <p class="red">-$1,009</p>
        <p class="grey">Today 1:32pm</p>
      </div>
    </div>
    <div class="transaction">
      <img src="@/assets/bitcoin.svg" alt="">
      <div class="flex-col">
        <p>Bitcoin</p>
        <p class="grey">Received</p>
      </div>
      <div class="flex-col">
        <p class="green">+$3,754</p>
        <p class="grey">Today 10:59am</p>
      </div>
    </div>
      <div class="transaction">
      <img src="@/assets/Etherum_icon.svg" alt="">
      <div class="flex-col">
        <p>Etherum</p>
        <p class="grey">Received</p>
      </div>
      <div class="flex-col">
        <p class="green">+$9,218</p>
        <p class="grey">Today 6:40am</p>
      </div>

    </div>
    <p class="asset-title">Assets</p>
    <div class="assets">
      <div class="flex-col asset-bitcoin">
          <img class="asset-icon" src="@/assets/bitcoin.svg" alt="">
          <p class="asset-money">Bitcoin</p>
          <div class="flex-row">
            <p class="asset-amount">121,6450.45</p>
            <p class="asset-abreviation">BTC</p>
          </div>
        </div>
      <div class="flex-col asset-etherum">
        <img class="asset-icon" src="@/assets/Etherum_icon.svg">
        <p class="asset-money">Etherum</p>
        <div class="flex-row">
          <p class="asset-amount">143,850.45</p>
          <p class="asset-abreviation">ETH</p>
        </div>

      </div>
    </div>
  </div>
</template>

<script>

</script>

<style>
.assets{
  display: flex;
  flex-wrap: wrap;
  gap:16px;
  align-items: center;
}
.asset-bitcoin{
  background: linear-gradient(98.73deg, #611D8D 35.75%, #2F7EC1 73.26%);
border-radius: 30px;
padding: 8px 24px;
display: flex;
flex-direction: column;
text-align: left;
justify-content:left;
width: 200px;
}
.asset-etherum{
  background: linear-gradient(99.56deg, #FAFF00 35.82%, #29ABE2 64.75%, rgba(255, 255, 255, 0.7) 91.33%);
border-radius: 30px;
padding: 8px 24px;
display: flex;
flex-direction: column;
text-align: left;
justify-content:left;
color: black;
width: 200px;
}
.right-info{
  /*position: absolute;
  left: 1345px;
  top: 240px;*/
  color: white;
}
.right-title{
  font-family: 'Poppins';
font-style: normal;
font-weight: 700;
font-size: 22px;
text-align: left;
padding-bottom: 24px;
}
.asset-title{
  font-family: 'Poppins';
font-style: normal;
font-weight: 700;
font-size: 22px;
text-align: left;
padding-bottom: 24px;
}
.transaction{
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 400px;
  padding-bottom: 16px;
  
}
.asset-icon{
  width: 48px;
}
.flex-col{
  display: flex;
  flex-direction: column;
  gap:8px;
}
.flex-row{
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
}
.transaction img{
  width: 32px;
}
.green{
  color:#4AD619;
}
.red{
  color: #D61919;
}

.grey{
  color: rgba(255,255,255,0.7)
}
@media(max-width: 1600px){
  .right-info{
    position:static;
    margin-left: 16px;
    margin-right: 16px;
  }
}
</style>