<template>
    <header>
        <nav class="nav_bg">
            <div class="nav_div1_bg">           
                <img src="../assets/mosa-ke-9853-240.png" alt="logo">
            </div>
            <div class="nav_div2_bg">
                <div class="nav_bg--button">                
                    <button class="nav_bg--button-bg" type="button"> {{writebutton}}</button>
                </div>
                <div class="nav_bg--ul--div">
                    <ul class="nav_bg--ul">
                        <li v-for="item in itens">{{item.name}}</li>
                    </ul>
                </div>
            </div>
        </nav>
    </header>
</template>

<script>
export default {
    data(){
        return{
            writebutton: 'Singup',
            itens: [
                {name: 'Home'},
                {name: 'Services'}, 
                {name: 'About is'},
                {name: 'Contact us'}
            ]
        }
    },
    methods:{

    },
}
</script>

<style scoped>
    header{
        top:0;
        left:0;
    }
    .nav_div1_bg img{
        display: flex;
        align-self: flex-start;
        transform: scale(0.8);
        transition: all 1s;
    }
    .nav_div1_bg img:hover{
        transform: scale(1);
        cursor:pointer;
    }
    .nav_div2_bg{
        margin-top:30px;
        margin-right: 60px;
    }
    .nav_bg{
        top:0;
        display:flex;
        justify-content: space-between;
    }

    .nav_bg--ul{
        display:flex;
        list-style: none;
        align-self: center;
    }

    .nav_bg--ul li{
        cursor: pointer;
        color:gray;
        margin:15px;
        font-family: 'PT Sans', sans-serif;
        transition: all 1s;
    }
    .nav_bg--ul li:hover{
        color:black;
    }
    /* div 2 */
    .nav_bg--ul--div{
        display: flex;
    }
    .nav_bg--button{
        display: flex;
        justify-content: flex-end;
    }

    .nav_bg--button-bg{
        cursor: pointer;
        border-radius:20px;
        color:gray;
        background:transparent;
        border:1px solid gray;
        padding:5px 10px;
        transition: all 1s;
    }

    .nav_bg--button-bg:hover{
        background:gray;
        color:white;
    }
</style>