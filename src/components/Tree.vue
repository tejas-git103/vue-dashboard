<template>
  <div class="tree-container">
      <div class="heading-bar">
          <div class="title">
              Tree
          </div>
          <div class="search-container">
              <img src="../assets/tree/search.png" class="search-icon">
              <input class="input" type="text" placeholder="Search Transaction Id">
          </div>
      </div>
      <div class="tree-legend">
          <img class="img-legend" src="../assets/tree/active.png">
          <img class="img-legend" src="../assets/tree/inactive.png">
          <img class="img-legend" src="../assets/tree/absent.png">
          <img class="img-legend" src="../assets/tree/block.png">
      </div>
      <div class="tree-root">
          <img class="img-root" src="../assets/tree/root.png">
      </div>
		<div class="connector-container-one">
			<span class="vertical-connector-one"></span>
			<span class="horizontal-conncetor-one"></span>
			<div class="child-connector-one">
				<span class="vertical-connector-one"></span>
				<span class="vertical-connector-one"></span> 
			</div>
		</div>
      <div class="tree-children">
          <img class="child invert" src="../assets/tree/active.png">
          <img class="child" src="../assets/tree/active.png">
      </div>
		<div class="row-two-connector">
			<div class="connector-container-two">
				<span class="vertical-connector-two"></span>
				<span class="horizontal-conncetor-two"></span>
				<div class="child-connector-two">
					<span class="vertical-connector-two"></span>
					<span class="vertical-connector-two"></span> 
				</div>
			</div>
			<div style="width:350px"></div>
			<div class="connector-container-two">
				<span class="vertical-connector-two"></span>
				<span class="horizontal-conncetor-two"></span>
				<div class="child-connector-two">
					<span class="vertical-connector-two"></span>
					<span class="vertical-connector-two"></span> 
				</div>
			</div>
		</div>
    <div class="tree-row-two">
		<div class="row-two-node">
			<img class="row-two-img" src="../assets/tree/purple.png">
			<img class="row-two-img-text" src='../assets/tree/purple_text.png'>
		</div>
		<div class="row-two-node">
			<img class="row-two-img" src="../assets/tree/purple.png">
			<img class="row-two-img-text" src='../assets/tree/purple_text.png'>
		</div><div class="row-two-node">
			<img class="row-two-img" src="../assets/tree/purple.png">
			<img class="row-two-img-text" src='../assets/tree/purple_text.png'>
		</div><div class="row-two-node">
			<img class="row-two-img" src="../assets/tree/purple.png">
			<img class="row-two-img-text" src='../assets/tree/purple_text.png'>
		</div>
    </div>
	<div class="row-three-connectors">
		<div class="connector-container-three">
				<span class="vertical-connector-three"></span>
				<span class="horizontal-conncetor-three"></span>
				<div class="child-connector-three">
					<span class="vertical-connector-three"></span>
					<span class="vertical-connector-three"></span> 
				</div>
		</div>
		<div class="connector-container-three">
				<span class="vertical-connector-three"></span>
				<span class="horizontal-conncetor-three"></span>
				<div class="child-connector-three">
					<span class="vertical-connector-three"></span>
					<span class="vertical-connector-three"></span> 
				</div>
		</div>
		<div class="connector-container-three">
				<span class="vertical-connector-three"></span>
				<span class="horizontal-conncetor-three"></span>
				<div class="child-connector-three">
					<span class="vertical-connector-three"></span>
					<span class="vertical-connector-three"></span> 
				</div>
		</div>
		<div class="connector-container-three">
				<span class="vertical-connector-three"></span>
				<span class="horizontal-conncetor-three"></span>
				<div class="child-connector-three">
					<span class="vertical-connector-three"></span>
					<span class="vertical-connector-three"></span> 
				</div>
		</div>

	</div>
	<div class="tree-row-three">
		<img class="row-three-img" src="../assets/tree/purple_text.png" >
		<img class="row-three-img" src="../assets/tree/purple_text.png" >
		<img class="row-three-img" src="../assets/tree/purple_text.png" >
		<img class="row-three-img" src="../assets/tree/purple_text.png" >
		<img class="row-three-img" src="../assets/tree/purple_text.png" >
		<img class="row-three-img" src="../assets/tree/purple_text.png" >
		<img class="row-three-img" src="../assets/tree/purple_text.png" >
		<img class="row-three-img" src="../assets/tree/purple_text.png" >
	</div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
.tree-container{
    width: 1598px;
    height: auto;
    background: #EAECFC 0% 0% no-repeat padding-box;
    border-radius: 56px;
    margin-top: 25px;
    margin-bottom: 25px;
    margin-left: 10px;
    margin-right: 10px;
    border-radius: 27px;
}
.heading-bar{
    padding: 50px;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    /* align-items: center; */

}
.title{
    font-size: 35px;
}
.search-container{
    display: flex;
    flex-direction: row;
    justify-content: start;
    padding: 15px;
    background: #FFFFFF 0% 0% no-repeat padding-box;
    box-shadow: 8px 8px 15px #1514571A;
    border-radius: 23px;
    width: 512px;
    /* height: 70px; */
}
.search-icon{
    width: 32px;
    height: 32px;
}
.input{
    font-size: 23px;
    border:none;
    height: 30px;
    width:auto;
    margin-left:20px;
    margin-right: 20px;
}
.input:focus{
    outline: none;
}

.tree-legend{
    display: flex;
    flex-direction: row;
    padding: 50px
}

.img-legend{
    width: 200px;
    height: 50px;
    margin-left: 15px;
    margin-right: 15px;
}

.tree-root{
    display: flex;
    flex-direction: row;
    justify-content: center;
}
.img-root{
    width: 250px;
    height: 250px;
}

.tree-children{
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
}
.child{
    width: 300px;
    /* height: 100px; */
}
.invert{
    transform: rotate(180deg);
}

.tree-row-two{
	display: flex;
	flex-direction: row;
	/* padding-top: 80px;	 */
	justify-content: space-evenly;
}

.row-two-img{
	height: 80px;
	width: 80px;
}
.row-two-node{
	display:flex;
	flex-direction: column;
	align-items: center;
}

.tree-row-three{
	display: flex;
	flex-direction: row;
	justify-content: space-evenly;
	/* padding-top: 50px; */
}

.row-three-img{
	height: 50px;
	/* width: 50px; */
}
.connector-container-one{
	display: flex;
	flex-direction: column;
	align-items: center;
}
.child-connector-one{
	display: flex;
	flex-direction: row;
	justify-content: space-between;
	width:700px;
}
.vertical-connector-one{
	border-left:1px grey solid ;
	height: 40px;
}
.horizontal-conncetor-one{
	border-bottom: 1px gray solid;
	width: 700px;
}
.row-two-connector{
	display: flex;
	flex-direction: row;
	justify-content: center;
}

.connector-container-two{
	display: flex;
	flex-direction: column;
	align-items: center;
}
.child-connector-two{
	display: flex;
	flex-direction: row;
	justify-content: space-between;
	width:350px;
}
.vertical-connector-two{
	border-left:1px grey solid ;
	height: 40px;
}
.horizontal-conncetor-two{
	border-bottom: 1px gray solid;
	width: 350px;
}

.row-three-connectors{
	display: flex;
	flex-direction: row;
	justify-content: space-evenly;
}
.connector-container-three{
	display: flex;
	flex-direction: column;
	align-items: center;
}
.child-connector-three{
	display: flex;
	flex-direction: row;
	justify-content: space-between;
	width:200px;
}
.vertical-connector-three{
	border-left:1px grey solid ;
	height: 40px;
}
.horizontal-conncetor-three{
	border-bottom: 1px gray solid;
	width: 200px;
}
</style>