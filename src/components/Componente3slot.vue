<template>
    <div class="componente3slotbg">
        <slot>
            <h1> {{titule1}} </h1>
            <img src="../assets/card7.jpg" alt="comic">

            <p> Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. </p>
            <div>
                redes sociais 
            </div>
        </slot>
    </div>
</template>

<script>
export default {
    data(){
        return{
            titule1: 'Marvel é o que há! '
        }
    }
}
</script>

<style lang="scss">
    @import '../sass/componente3slot.scss'
</style>
