<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <p><a href="http://www.w3school.com.cn" id="w3s">W3School.com.cn</a></p>
    <button @click="jqueryDemo">显示 href 值</button>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import $ from 'jquery';
export default {
  name: 'Home',
  components: {
    HelloWorld
  },
  methods:{
    jqueryDemo() {
      console.log('2333')
      alert($("#w3s").attr("href"));
    }
  },
}
</script>
