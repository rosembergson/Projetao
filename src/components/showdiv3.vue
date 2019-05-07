<template>
    <div class="div3_bg-bg">
        <div class="div3_bg">
            <div class="div3_bg--formas">
                <img src="../assets/hockey-lgoo.png" alt="logo">
            </div>
            <div class="div3_bg--show">
                <div>
                    <h1>Everything your business needs</h1>
                    <p> We offer everything you need from incorporation to filings for corporate actions. As your business grows, we will be by your side to help you do paperwork efficiently. </p>
                    <button>Learn More</button>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
    .div_bg-bg{
        width:100%;
        margin:0;
    }
    .div3_bg{
        width:85%;
        display:flex;
        height: 460px;
        border-bottom-right-radius:100px;
        background-color:#2e3038;
        
    }
    .div3_bg--formas {
        display:flex;
        justify-content:center;
        width:50%;
        height:100%;
    }
    .div3_bg--formas img{
        width:300px;
        display:flex;
        align-self:center;
        height:70%;
        animation: example 4s infinite;
    }
    .div3_bg--show{
        color:white;
        display:flex;
        justify-content:center;
        width:30%;
    }
    .div3_bg--show h1{
        font-family: 'Playfair Display', serif; 
        font-size:40px;
        color:#ff4a5a;
    }
    .div3_bg--show p{
        font-family: 'Muli', sans-serif;
        font-size:16px;
    }

    .div3_bg--show div{
        align-self:center;
    }

    .div3_bg--show button{
        cursor:pointer;
        background:#ff4a5a;
        padding:10px 25px;
        border-radius:20px;
        border:none;
        color:white;
    }
    .div3_bg--show button:hover{
        animation: button 2s infinite;
    }
    /* animation */

    @keyframes example {
        0%{
            
        }
        50% {
            transform: translateY(20px);
        }

        100%{
            transform: translateY(0px);
        }
    }

    @keyframes button{
        0%{

        }
        50%{
            transform: scale(0.95);
        }
        100%{
            transform: scale(1);
        }
    }
</style>