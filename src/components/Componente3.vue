<template>
    <div class="componente3bg">
            <div>
                <componente3slot>
                <slot></slot>
                </componente3slot>
            </div>
    </div>
</template>

<script>

import Componente3slot from './Componente3slot'
export default {
    data(){
        return{
            titule1: 'Cara Comum',

        }
    },
    components:{
        'componente3slot' : Componente3slot
    }
}
</script>


<style lang="scss">
    @import '../sass/componente3slot.scss'
</style>