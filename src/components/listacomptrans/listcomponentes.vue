<template>
    <div class="liscomponentsbg1">
        <h2> Menu Componentes </h2>

        <div class="listcomponentes_adicionar">
            <input type="text" placeholder="Insira seu component novo" @keyup.enter="adicionar" ref="input ">
        </div>
        
        <section class="listcomponentesbg2">
            <transition-group tag="ul" class="listcomponentesbg2_ul">
                <li v-for="(tecnologia, indice) in tecnologias" :key="tecnologia">
                    <span>{{ tecnologia }} </span>
                    <button type="button" @click="remove(indice)"> x </button>
                </li>
            </transition-group>
        </section>
    </div>

</template>

<script>
export default {
    data(){
        return{
            tecnologias:[
                'Vue.js',
                'Vuex.js',
                'Angular',
                'Jquery',
                'React',
                'React Native'
            ]
        }
    },
    methods:{
        adicionar(event){
            const newitem = event.target.value
            if(newitem) {
                const indice = Math.floor(Math.random()*this.tecnologias.length)
                this.tecnologias.splice(indice,0,newitem)
                this.$ref.input.value= ''
            }
        },
        remove(indice){
            this.tecnologias.splice(indice, 1)
        }
    }
}
</script>

<style lang="scss">
    @import "../../sass/listcomponnents.scss";
    @import "../../sass/animation.scss"
</style>