<template>
  <div id="app">
    <router-view></router-view>
  </div>
</template>

<script lang="ts">
import * as firebase from "firebase";
import { Component, Vue } from "vue-property-decorator";
import HelloWorld from "./components/HelloWorld.vue";

@Component({
  components: {
    HelloWorld
  },
  mounted() {
    const firebaseConfig = {
      apiKey: "AIzaSyBScxeAtzEu5HV91vLHe9aKDXiXAO8GOhg",
      authDomain: "order-helper-2fdd0.firebaseapp.com",
      databaseURL: "https://order-helper-2fdd0.firebaseio.com",
      projectId: "order-helper-2fdd0",
      storageBucket: "order-helper-2fdd0.appspot.com",
      messagingSenderId: "745560926469",
      appId: "1:745560926469:web:c37f086c6d87d507162f6c",
      measurementId: "G-2H42ZEYKP5"
    };
    // Initialize Firebase
    firebase.initializeApp(firebaseConfig);
    firebase.analytics();
  }
})
export default class App extends Vue {}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
