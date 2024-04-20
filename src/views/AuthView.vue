<template>
    <div class="main">
        <div class="main-auth">
            <div class="title">
                <h3>Login de usuario</h3>
            </div>
        <div class="main-form">
            <form action="">
                <div class="form-input">
                    <label for="user">User</label>
                    <input type="text" required name="user" class="form-control">
                </div>
                <div class="form-input">
                    <label for="password" class="">Password</label>
                    <input type="text" required name="password">
                </div>
                <div class="form-controls">
                    <input type="submit" value="Login">
                    <router-link :to="{name:'forgot-password'}">Não tem uma conta, se-cadastre</router-link>
                </div>
            </form>
        </div>
        </div>
    </div>
</template>

<script>
    export default {
        name:"AuthView"
    }
</script>

<style lang="scss" scoped>
@import '../styles/global.scss';
    .main-auth{
       border: solid 1px $color-1;
       border-radius: 4px;
       margin: 0 auto;
       padding: 2em;
    }
    .title{
        color:$color-1;
        font-family: $ff-roboto;
        font-size: 14px;
        font-weight: bolder;  
        text-align: center;
        margin-bottom: 15px;
        padding: 1em;
    }

    .main-form{
        border:none;
        display: block;
    }

    .form-input{
        margin: 12px 0px;
        display: flex;
        flex-direction: column;
    }

    .form-input label{
        font-size: 12px;
        font-family: $ff-roboto;
        font-weight: 500;
        color: $color-5;
        margin-bottom: 5px;
    }

    .form-input input:not(input[type="submit"]){
        color: $color-5;
        padding: 5px;
        border: solid 1px $color-1;
        border-radius: 4px;
        font-size: 13px;
    }
    
    .form-controls{
        width: 100%;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        margin-top: 10px;
        padding: 1em;
    }

    .form-controls input{
        padding: 10px 12px;
        border: none;
        border-radius: 8px;
        background: $color-5;
        color: $text-color;
        font-weight: 700;
        font-size: 13px;
        margin-bottom: 1em;
        cursor: pointer;
        
    }

    .form-controls input:hover{
        padding: 10px 12px;
        border: none;
        border-radius: 8px;
        background: $color-3;        
    }
   
    .form-controls a{
        text-decoration: none;
        font-size: 12px;
        font-family: $ff-ubuntu;
        color: $color-2;
        text-align: center;
    }

</style>