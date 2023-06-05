<template>
   <div class="container">
    <div class="box">
        <h3 class="heading">Premium Earned</h3>
        <span class="amount">$ 50125</span>
    </div>
    <div class="box">
        <h3 class="heading">Premium Earned</h3>
        <span class="amount">$ 50125</span>
    </div>
    <div class="box">
        <h3 class="heading">Premium Earned</h3>
        <span class="amount">$ 50125</span>
    </div>
    <div class="box">
        <h3 class="heading">Premium Earned</h3>
        <span class="amount">$ 50125</span>
    </div>
   </div>
</template>

<style scoped>
.container {
    border: 2px solid red;
    min-height: 20vh;
    width: 100%;
    display: flex;
    align-items: center;
    padding: 10px;
    justify-content: space-between;
  }
  .box{
    height: 90%;
    width: 24%;
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
    border-radius: 10px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 10px;
  }
  .heading{
font-size: 1.7rem;
color: green;
letter-spacing: 1px;
  }
  .amount{
    height: 90px;
    width: 90px;
    border: 1px solid green;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 50%;
    font-size: 1.2rem;
    font-weight: bold;
    color: white;
    background-color: green ;
  }
  

  </style>