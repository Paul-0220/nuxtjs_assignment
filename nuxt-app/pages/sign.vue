<template>
<fieldset>
    <legend>
        <h2>SignUp</h2>
    </legend>
    <form id="signUp">
        <input type="text" id="userName" v-model="name" name="userName" placeholder="User Name"><br><br>
                <input type="email" id="email" v-model="email" name="email" placeholder="Email"><br><br>
                        <input type="password" id="password" v-model="password" name="password" placeholder="password"><br><br>
                        <button @click="sign">Sign Up</button>
    </form>
</fieldset>
</template>
<script>
 import axios from 'axios'
 import indexVue from "./index.vue";
 export default {
    name:"sign",
    data(){
         return {
            name:'',
            email:'',
            password:'',
        }
     },
    methods:{
         async sign(){
             console.log('signUp',this.name,this.email,this.password)
             let result=await axios.post('http://localhost:3000/user',{
                 name:this.name,
                 email:this.email,
                 password:this.password
             })
         }
     }
 }
</script>
<style>
#signUp input{
width: 300px;
height: 40px;
padding-left: 20px;
margin-bottom: 30px;
margin-left: auto;
margin-right: auto;
border:1px solid skyblue
}
#signUp button {
    width: 320px;
    height: 40px;
    border: 1px solid skyblue;
    color: #fff;
    background-color: skyblue;
    cursor: pointer;
}
</style>