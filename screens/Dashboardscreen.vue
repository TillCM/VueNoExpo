<template>

     <view class ="container" >
     <image class = "logo"
          :source="require('./teamfusmall.png')"
        />
     <text class ="heading2">Login</text>

   

    </view>
   
</template>

<style scoped>

.logo{
position: absolute;
width: 34px;
height: 40px;
left: 161px;
top: 147px;

}

.heading2{
position: absolute;
top: 200px;
left: 161px;
font-family: Poppins;
font-style: normal;
font-weight: 600;
font-size: 30px;
line-height: 45px;
display: flex;
align-items: center;
text-align: center;
}



.container{
flex:1;
position: relative;
width: 360px;
height: 640px;

background-color: #FFFFFF;
}


</style>