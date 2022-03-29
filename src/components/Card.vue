<template>
  <div class="card-container">
        <div class="card-logo">
            <slot name="logo"></slot>
            <slot name="graph"></slot>
        </div>
        <div class="card-text">
            <div class="text-title">{{title}}</div>
            <div class="text-value">{{value}}</div>
        </div>
    </div>
</template>

<script>
export default {
    props:{
        title:String,
        value:String,
    }
}
</script>

<style>

.card-container{
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    width: 340px;
    height: 214px;
    background: #EFF2FE 0% 0% no-repeat padding-box;
    box-shadow: 8px 8px 18px #04044345; 
    margin-left: 25px;
    margin-right: 25px;
    border-radius: 27px;
}
.card-logo{
    /* margin: 20px; */
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
}

.logo{
    width: 60px;
    height: 60px;
}

.graph{
    height: 60px;
    width: 160px;
}

.card-text{
    display: flex;
    flex-direction: column;
    margin-left: 25px;
}

.text-title{
    color:#535C70;
    font-size: 17px;
}
.text-value{
    color: #2A3141;
    font-size: 31px;
}
</style>