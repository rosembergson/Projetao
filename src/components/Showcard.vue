<template>
    <div class="showcard">
        <ul class="showcardbg">
            <!-- card -->
            <li class="showcardbg_cards" v-for="card in cards" :key="card.id">
                <div class="cards--img">
                    <img :src="card.code" alt="city1">
                    <span> photos </span>
                </div>
                <h3 class="cards--titule3"> {{ card.titule1 }} </h3>
                <h6 class="cards--titule6"> {{ card.qualif }} </h6>
                <button @click="addFilme" :card ="car" class="cards--button" type="button"> Add </button>
                <ul class="cards--dates">  
                    <li>6 months</li>
                    <li>13:00 PM</li>
                </ul>
                <p>{{f}}</p>
            </li>
        <!-- last card -->
        </ul>
    </div>
</template>

<script>
export default {
    data(){
        return{
            car: undefined,
            cards:[
                {id:1 , titule1: 'City New York', qualif: 'Is beautiful city with more', code:require('../assets/cardimage1.jpg')},
                {id:2 , titule1: 'City São Paulo', qualif: 'Is ungly city with more trash', code:require('../assets/cardimage2.jpg')},
                {id:3 , titule1: 'City Hong Kong', qualif: 'Is big city with more Chineses', code:require('../assets/cardimage3.jpg')},
                {id:4 , titule1: 'City Madrid', qualif: 'Is beautiful city with more bull',  code:require('../assets/cardimage4.jpg')},
            ]
        }
    },
    methods:{
        addFilme($event){
            this.car = this.card
        }
    }
}
</script>

<style lang="scss">
    @import "../sass/Showcard.scss";
</style>