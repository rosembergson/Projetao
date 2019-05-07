<template>
    <li class="componentecard2bg">
        <div class="componentecard2bg_img">
            <img :src="Card.code" alt="Card.alt">
            <span></span>
        </div>
        <h3 class="componentecard2bg_titule3">{{Card.titule3}}</h3>
        <h6 class="componentecard2bg_titule6">{{Card.titule6}}</h6>

        <button type="button" class="componentecard2bg_buttonadd">{{buttonselect}}</button>
    </li>
</template>

<script>
export default {
    data(){
        return{
            buttonselect: 'Select'
        }
    },
    props:{
        Card:{
            type: Object,
            required:true,
        }
    }
}
</script>

<style lang="scss">
    @import '../sass/Cardstyle.scss'
</style>