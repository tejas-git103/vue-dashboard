<template>
  <div class="menu-container">
      <div class="menu-title">
          Menu
      </div>
      <div class="menu-list" >
          <div :class="selection == 'home'?'list-item selected':'list-item'" @click="$emit('emitSelection','home')">
                <img v-if="selection == 'home'" class="list-img" src="../assets/menu/Home_s.png" />
                <img v-else class="list-img" src="../assets/menu/Home.png" />
                <div class="list-title">Home</div>
          </div>
          <div class="list-item">
                <img  class="list-img" src="../assets/menu/Invest_wallet.png" />
                <div class="list-title">Invest Wallet</div>
          </div>
          <div class="list-item">
                <img class="list-img" src="../assets/menu/Reports.png" />
                <div class="list-title">Reports</div>
          </div>
          <div :class="selection == 'tree'?'list-item selected':'list-item'" @click="$emit('emitSelection','tree')">
                <img v-if="selection == 'tree'" class="list-img" src="../assets/menu/Team_s.png" />
                <img v-else class="list-img" src="../assets/menu/Team.png" />
                <div class="list-title">Team</div>
          </div>
          <div class="list-item">
                <img class="list-img" src="../assets/menu/Income.png" />
                <div class="list-title">Income</div>
          </div>
          <div class="list-item">
                <img class="list-img" src="../assets/menu/Withdrawal.png" />
                <div class="list-title">Withdrawal</div>
          </div>
      </div>
      <div class="path">
          <img src="../assets/menu/referral_link.svg">
      </div>
  </div>
</template>

<script>
export default {
    props:{
        selection:String
    }
}
</script>

<style>
.menu-container{
    display: flex;
    flex-direction: column;
    max-width: 272px;
    height:max-content;
    background: #F6F6FF 0% 0% no-repeat padding-box;
    box-shadow: 10px 10px 15px #15145724;
    border-radius: 56px;
    padding: 40px;
    margin-top: 25px;
    margin-bottom: 25px;
    margin-left: 10px;
    margin-right: 10px;
}

.menu-title{
    font-size: 25px;
    font-weight: bold;
    margin-top: 30px;
    margin-bottom: 30px;
}

.menu-list{
    display: flex;
    flex-direction: column;
}
.list-item {
    display: flex;
    flex-direction: row;
    justify-content:flex-start;
    margin-top: 30px;
    margin-bottom: 30px;
}
.list-title{
    font-size: 25px;
    margin-left: 20px;
    /* color: #213141; */
}
.selected{
    color: #5221f3;
}
.list-img {
    width: 30px;
    height: 30px;
    color: #522153;
}
.path{
    height: 180px;
    width: 200px;
    background:transparent url('../assets/menu/Path62774.png') 60% 60% no-repeat padding-box;
    padding-left: 20px;
    padding-top: 30px;
}
</style>