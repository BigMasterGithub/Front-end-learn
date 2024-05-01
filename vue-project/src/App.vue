<!-- 声明式构建API -->
<!-- <script >
    export default{
      date(){
        return{
          msg:"上海"
        }
      }
    }
</script> -->
<!-- 组合式构建API 推荐使用！ -->
<script setup>
    import {ref} from 'vue'
     import APIVUE from "./components/api.vue" ;
    
     import UserVUE from "./componets/Userinfo.vue";
    //调用ref函数，定义响应式数据
    const msg = ref("西安")    
    


</script>


<template>

  <h1>{{msg}}</h1>
  <br/>

  <APIVUE/>
  <UserVUE></UserVUE>
</template>

<style scoped>
  h1{
    color:yellow
  }
</style>
