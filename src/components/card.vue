<template>
    <div class="div_card">
    <h1> Why Caxis? </h1>
        <div class="card">
            <div v-for="item in itens" class="card_bg">
                <h4>{{item.titule}}</h4>
                <p>{{item.parf}}</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
            itens:[
                {titule: 'Fast', parf: 'We use technology wherever possible to serve you efficiently.'},
                {titule: 'Easy', parf:'We will be with you every step of the way to guide you through the process.'},
                {titule: 'Affordable', parf: 'Technology allows us to stay nimble. You will always get the best value with us.'},
                {titule: 'Legal Suporte', parf: 'We offer free legal & tax consultations to help you run your business.'},
            ]
        }
    },
}
</script>

<style scoped>

.div_card{
    width:60%;
    position: relative;
}
.div_card:before{
    opacity: 0.3;
    content: '';
    width: 100%;
    height: 100%;
    position: absolute;
    left: 0;
    top: 0;
    background-image: url("../assets/Online-Survey-Tool.png");
    background-position: center;
    background-repeat: no-repeat;
    background-size: contain;
}
.div_card h1{
    text-align:center;
    font-size:48px;
    font-family: 'Playfair Display', serif; 
    opacity: 0.8;
}
.card{
    display:flex;
    justify-content: space-evenly;
    flex-wrap:wrap;
    width:100%;
    margin:0;
    
}
    .card_bg{
        width:40%;
        padding:20px;
        font-family: 'Muli', sans-serif;
    }

    .card_bg h4{
        font-family: 'Muli', sans-serif;
        color:#ff4a5a;
    }

    .card_bg p{
        color:black;
        
    }
</style>