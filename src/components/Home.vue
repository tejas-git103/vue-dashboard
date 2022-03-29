<template>
<div class="dashboard-container">
    <hr/>
    <div class="title">Dashboard</div>
    <div class="row-one">
        <Card :title="'ROI Income'" :value="'4280.884 TRX'">
            <template #logo>
                <img class="logo" src="../assets/roi_income-logo.png">
            </template>
            <template #graph>
                <img class="card-graph" src="../assets/roi_income.png" >
            </template>
        </Card>
        <Card :title="'Direct Income'" :value="'132.720 TRX'">
            <template #logo>
               <img class="logo" src="../assets/direct_income-logo.png" >
            </template>
            <template #graph>
                <img class="card-graph" src="../assets/direct_income.png" >
            </template>
        </Card>
        <Card :title="'Binary Income'" :value="'57.840 TRX'">
            <template #logo>
                <img class="logo" src="../assets/binary_income_logo.png">
            </template>
            <template #graph>
                <img class="card-graph" src="../assets/binary_income.png" >
            </template>
        </Card>
        <Card :title="'Current Earning limit'" :value="'14460 TRX'">
            <template #logo>
                <img class="logo" src="../assets/current_earning_limit-logo.png">
            </template>
            <template #graph>
                <img class="card-graph" src="../assets/current_earning_limit.png" >
            </template>
        </Card>
    </div>
    <div class="row-two">
        <div class="roi">
            <div style="text-align:center">
                <div class="roi-title">ROI</div>
                <div class="roi-content">(Retopup Reminder)</div>
            </div>
            <img class="watch" src="../assets/watch.png">
        </div>
        <div class="my-total-earning">
            <div class="cards">
                <Card :title="'Total Active Deposits'" :value="'348 TRX'">
                    <template #logo>
                        <img class="logo" src="../assets/total_active_deposits.png">
                    </template>  
                </Card>
                <Card :title="'Total Withdrawal'" :value="'3615.00 TRX'">
                    <template #logo>
                        <img class="logo" src="../assets/total_withdrawal.png">
                    </template>
                </Card>
            </div>
            <div class="total-earn-graph">
                <div>
                    <div class="my-earning-title">My Total Earning</div>
                    <div class="my-earning-content">4471.440 TRX</div>
                </div>
                <img src="../assets/my_total_earning.png" class="total-earn-img">
            </div>
        </div>
    </div>
    <div class="buttons-container">
        <button class="btn">Add Fund</button>
        <button class="btn">Withdraw </button>
    </div>
    <div class="graph-container">
        <div class="graph">
            <img src="../assets/graph.png">
        </div>
    </div>
</div>
</template>

<script>
import Card from './Card.vue'
export default {
components:{
    Card
}
}
</script>

<style>
.dashboard-container{
    display: flex;
    flex-direction: column;
    justify-content: start;
    width: 1598px;
    /* height: 2216px; */
    background: #EAECFC 0% 0% no-repeat padding-box;
    border-radius: 56px;
    margin-top: 25px;
    margin-bottom: 25px;
    margin-left: 10px;
    margin-right: 10px;
    border-radius: 27px;
}

.row-one{
    display: flex;
    flex-direction: row;
    /* background-color: aqua; */
    margin-top: 25px;
    margin-bottom: 25px;
}

.row-two{
    display: flex;
    flex-direction: row;
    /* background-color: aqua; */
    margin-top: 25px;
    margin-bottom: 25px;
}

.buttons-container{
    display: flex;
    flex-direction: row;
    /* background-color: aqua; */
    margin-top: 25px;
    margin-bottom: 25px;
}

.graph-container{
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    width: 1503px;
    height: 759px;
    background-color: white;
    margin-top: 25px;
    margin-bottom: 25px;
    margin-left: 25px;
    border-radius: 56px;
}

.title{
    font-size: 31px;
    font-weight: bold;
    margin-left: 25px;
    margin-top: 25px;
}

.roi{
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    align-items: center;
    height: 578px;
    width: 341px;
    background:transparent linear-gradient(180deg, #4D24F3 0%, #7F08F6 100%) 0% 0% no-repeat padding-box;
    box-shadow: inset -8px -8px 16px #551FF3;
    margin-left: 25px;
    margin-right: 25px;
    border-radius: 27px;
}
.my-total-earning{
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
    height: 578px;
    width: 1114px;
    margin-left: 25px;
    margin-right: 25px;
    background: #DBDCF0 0% 0% no-repeat padding-box;
    border-radius: 27px;
}

.btn{
    width: 727px;
    height: 78px;
    background: transparent linear-gradient(102deg, #73BBEA 0%, #5654E6 100%) 0% 0% no-repeat padding-box;
    box-shadow: 8px 8px 16px #211F8F33;
    font-size:31px;
    color: white;
    border-radius: 19px;
    margin-left: 25px;
    margin-right: 25px;
    border-radius: 19px;
}

.logo{
    width: 60px;
    height: 60px;
}

.card-graph{
    height: 60px;
    width: 160px;
}

.watch{
    height: 200px;
    width: 200px;
}
.roi-title{
    color: white;
    font-size: 40px;
    font-weight: bold;
}
.roi-content{
    color: white;
    font-size: 31px;
}

.cards{
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
}

.total-earn-graph{
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;

}

.total-earn-img{
    height: 300px;
    width: 560px;
}
.my-earning-title{
    color: black;
    font-weight: bold;
    font-size: 26px;
}

.my-earning-content{
    color: #535C70;
    font-size: 26px;
}

.graph{
    width: 1292px;
    height: 514px;
}
</style>