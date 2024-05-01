<!--使用组合式API -->
<script setup>
        import {ref} from 'vue'
        import axios from 'axios'

        axios.get().then().catch(err=>{
            console.log(err);
        })

        const data = ref(){
            return{
                searchName:''
            }
        }

        const methods = ref(){
            return {
                search():{

                }
            }
        }
</script>
    

<template>
  <div id="app">
        <!-- 用户名 <input type="text" v-model="xx">        
        <button v-on:click="search">搜索</button> -->
        <br />
        <br />
        <table border="1 sold" colspa="0" cellspacing="0">
            <tr>
                <th>id</th>
                <th>用户名</th>
                <th>密码</th>
                <th>昵称</th>
                <th>注册时间</th>
            </tr>
            <!-- <tr v-for="(curuser,index) in list"> -->
                <td>{{curuser.id}}</td>
                <td>{{curuser.username}}</td>
                <td>{{curuser.password}}</td>
                <td>{{curuser.nickname}}</td>
                <td>{{curuser.signtime}}</td>
            <!-- </tr> -->


        </table>


    </div>


</template>