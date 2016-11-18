<template>
    <div class="container">        
        <div class="row">
            <div class="col m4 offset-m4 ">                    
                    <h2 class="center-align">
                        <img src="../../img/laracounts.png" class="responsive-img">
                    </h2>               
                    
                    <div class="row">
                        <form>
                            <div class="row">
                                <div class="input-field col s12">
                                    <input type="email" id="email" v-model="user.email">
                                    <label for="email">E-mail:</label>
                                </div>
                            </div>
                            <div class="row">
                                <div class="input-field col s12">
                                    <input type="password" id="pass" v-model="user.password">
                                    <label for="pass">Senha:</label>
                                </div>
                            </div>
                            <div class="row">
                                <div class="col m12">
                                    <p class="center-align">
                                        <button class="btn btn-large btn-default" type="button" @click="login()">Entrar</button>
                                    </p>
                                </div>
                            </div>
                        </form>                    
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default{
        data(){
            return{
                user:{
                    email:'',
                    password:''
                }
            };
        },
        ready(){
            console.log('Component ok');
        },

        methods:{
            login(){
                console.log('Login Funcionando');
            }
        }
    }

</script>