<template>
<fieldset>
    <legend>
        <h2>LogIn</h2>
    </legend>
    <form id="logIn">
        <input type="email" id="email" name="email" placeholder="Email"><br><br>
        <input type="password" id="password" name="password" placeholder="password"><br><br>
        <button @click="logIn">LogIn</button>
    </form>
</fieldset>
</template>
<script></script>
<style>
#logIn input{
    width: 300px;
    height: 40px;
    padding-left: 20px;
    margin-bottom: 30px;
    margin-left: auto;
    margin-right: auto;
    border: 1px solid skyblue;
}
#logIn button{
    width: 320px;
    height: 40px;
    border: 1px solid skyblue;
    color: #fff;
    background-color: skyblue;
    cursor: pointer;
}</style>
