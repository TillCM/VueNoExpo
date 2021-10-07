<template>

     <view class ="container" >
     <image class = "logo"
          :source="require('./teamfusmall.png')"
        />
     <text class ="heading2">Login</text>

    <text-input class ="email"
        v-model="text"
      />

       <text-input class ="password"
        
        v-model="text"
      />

      
       <button 
        @press="changeRoute"
        title="login"
        class ="loginbtn"
        accessibility-label="Press to login to teamfu"
      
    />


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

.email{

  height: 40px;
  display: flex;
  width : 300px;
  top: 270px;
  left: 35px;
  border-color: #333E55;
  border-width: 1;
  border-radius:  6px;
  padding : 10;
}

.password{

  height: 40px;
  display: flex;
  width : 300px;
  top: 290px;
  left: 35px;
  border-color: #333E55;
  border-width: 1;
  border-radius:  6px;
  padding : 10;
}

.loginbtn
{
  height: 40px;
  display: flex;
  width : 300px;
  top: 320px;
  left: 35px;
  border-color: #333E55;
  border-width: 1;
  border-radius:  6px;
  padding : 10;
}


.container{
flex:1;
position: relative;
width: 360px;
height: 800px;

background-color: #FFFFFF;
}



</style>

<script>
export default {
  props: {
    navigation: { type: Object }
  },
  methods: {
    changeRoute() {
      this.navigation.navigate('Dashboard');
    }
  }
}
</script>


