<template>
  <div class="header" text-align:center>

    <span class="text">股票交易系统</span>

  </div>
</template>

<script>


export default {
    name:"TopBar",
    data(){
      return {
      }
    },

    methods: {
    }
}
</script>

<style type="text/css">
.header{
    height:100px;
    background:-webkit-linear-gradient(bottom,#fcaf56,#ffedd8);
    border-radius: 4px
}
.text{
    color: #250;
    font-size: 25px;
    margin-top:40px;
    height: 100px;
	line-height: 100px;
}
</style>
