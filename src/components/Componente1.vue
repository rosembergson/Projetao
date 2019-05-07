<template>
<div>
    <div class="componente1bg">
        <!-- Escolha o button para renderizar seu componente -->

        <!--  Form principal -->
        <form action="POST" class="componente1bg_form">
            <label> Nome: <input class="form--inp" type="text" v-model="desenvolvedor.name"></label>
            <label> Sobrenome: <input class="form--inp" type="text" v-model="desenvolvedor.sobrenome"></label>
            <label> Email: <input class="form--inp" type="email" v-model="desenvolvedor.email"></label>
            <label> Idade: <input class="form--inp" type="text" v-model="desenvolvedor.idade"></label>
            <label> Gênero: 
                <input type="radio" name="gender" value="male"> Male
                <input type="radio" name="gender" value="female"> Female
            </label>

            <label class="componente1bg_labellast">
            Cidade: 
                <select v-model="desenvolvedor.cidade" class="form--select" name="Select" >
                    <option value="Select" selected> --- </option>
                    <option value="Canindé">Canindé</option>
                    <option value="Caridade">Caridade</option>
                    <option value="Quixadá">Quixadá</option>
                    <option value="Jaguaretama">Jaguaretama</option>
                    <option value="Paramoti">Paramoti</option>
                    <option value="Barbalha">Barbalha</option>
                    <option value="Fortaleza">Fortaleza</option>    
                </select> 
            </label>
            <button class="button1bg"> Envia </button>
        </form>
    </div>
</div>
</template>


<script>
export default {
    data(){
        return{
            desenvolvedor:{
                name:'',
                sobrenome:'',
                email:'',
                idade:'',
                genero:'',
                cidade:'',
            }
        }
    }
}
</script>

<style lang="scss">
    @import "../sass/form.scss"
</style>