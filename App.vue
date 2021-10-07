<template>
<app-navigator></app-navigator>
</template>



<script>
import{
  createAppContainer,
  createStackNavigator,
  createDrawerNavigator
}from "vue-native-router";



import LoginScreen from "./screens/LoginScreen.vue";
import Dashboard from "./screens/Dashboardscreen.vue";

const DrawerNavigator = createDrawerNavigator(
  {
    Login: LoginScreen,
    Dashboard:Dashboard
  },
  {
    initialRouteName: 'Login'
  }
);

const StackNavigator = createStackNavigator(
  {
    Drawer: DrawerNavigator,
    Login: LoginScreen,
    Dashboard:Dashboard
    
  },
  {
    initialRouteName: 'Login'
  });

const AppNavigator = createAppContainer(StackNavigator);

export default {
  components: { AppNavigator }
}
</script>


