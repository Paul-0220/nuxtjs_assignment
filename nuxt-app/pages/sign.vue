<template>
<fieldset>
    <legend>
        <h2>SignUp</h2>
    </legend>
    <form id="signUp">
        <input type="text" id="userName" name="userName" placeholder="User Name"><br><br>
                <input type="email" id="email" name="email" placeholder="Email"><br><br>
                        <input type="password" id="password" name="password" placeholder="password"><br><br>
                        <button>Sign Up</button>
    </form>
</fieldset>
</template>
<script></script>
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