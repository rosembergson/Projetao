<template>
    <div>
        <h2> {{namesection }}</h2>
        <div class="componente2bg">
            <compcard v-for="card in cards" :Card="card" :key="card.id" />
        </div>
    </div>
</template>

<script>

import Componente2card from './Componente2.vue'

export default {
    components:{
        'compcard' : Componente2card
    },
    data(){
        return{
            namesection: 'Card List',
            cards:[
                {id:1 , code:require('../assets/cardimage1.jpg'), titule3:'City Canindé', titule6:'Lorem Ipsum is simply dummy text of the printing and typesetting industry. ', alt:'city1'},
                {id:2 , code:require('../assets/cardimage2.jpg'), titule3:'City Caridade', titule6:'Lorem Ipsum is simply dummy text of the printing and typesetting industry. ',alt:'city2'},
                {id:3 , code:require('../assets/cardimage3.jpg'), titule3:'City Paramoti', titule6:'Lorem Ipsum is simply dummy text of the printing and typesetting industry. ',alt:'city3'},
                {id:4 , code:require('../assets/cardimage4.jpg'), titule3:'City Quixadá', titule6:'Lorem Ipsum is simply dummy text of the printing and typesetting industry. ',alt:'city4'},
                {id:5 , code:require('../assets/cardimage5.jpg'), titule3:'City Quixeramobim', titule6:'Lorem Ipsum is simply dummy text of the printing and typesetting industry. ',alt:'city5'},
                {id:6 , code:require('../assets/cardimage6.jpg'), titule3:'City Barbalha', titule6:'Lorem Ipsum is simply dummy text of the printing and typesetting industry. ',alt:'city6'}
            ]
        }
    }
}
</script>

<style lang="scss">
    
</style>