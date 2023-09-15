<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
function autourl() {
  // console.log("ggggg");
  console.log(navigator.userAgent);
  // if(navigator.userAgent.includes("facebook")){
       window.location.href = "https://server-deeplink-ausi4.vercel.app/";
  //  }
  // window.open("https://server-deeplink-ausi4.vercel.app/","_self");
}
autourl()

</script>

<template>
  <h1>{{ msg }}</h1>

  <div class="card">
    <button type="button" @click="count++">count is {{ count }}</button>
    <p>
      Edit
      <code>components/HelloWorld.vue</code> to test HMR
    </p>
  </div>

  <p>
    Install
    <a href="https://server-deeplink-ausi4.vercel.app/" target="_blank">Volar</a>
    in your IDE for a better DX
  </p>
  <p class="read-the-docs">Click on the Vite and Vue logos to learn more</p>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
