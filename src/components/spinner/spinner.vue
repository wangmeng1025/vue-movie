<template>
  <div class="loader">
	   <div class="loader2">
	     <i></i>
	     <i></i>
	     
	   </div>
	</div>
</template>

<script>
  export default {
  }
</script>

<style>
	 .loader{
  	    width: 100%;
  	    height: 200px;
  	    float: left;
  	    box-sizing: border-box;
  	    display: flex;
  	    align-items: center;
  	    justify-content: center;
  }
   @-webkit-keyframes loader2{
  	0%{
      transform: rotate(0deg)
    }
    100%{
      transform: rotate(360deg);
    }
  }
  .loader2{
    width: 40px;height: 40px;
    position: relative;
  }
  .loader2 i{
  	     display: block;
  	     float: left;
  	     margin-right: 6px;
  	     border: 2px solid #df2d2d;
         border-color: transparent #df2d2d;
  	     border-radius:50%;
         position: absolute;
         animation: loader2 0.5s linear 0s infinite
  	    
  }

  .loader2 i:first-child{
  	   width: 70px;
       height: 70px;
       top: 0;
       left: 0;
  }
  .loader2 i:last-child{
       width: 40px;
       height: 40px;
       top: 15px;
       left: 15px;
       animation: loader2 0.5s linear 0.2s infinite reverse
  }

</style>
