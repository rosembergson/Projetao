<template>
<section class="main2_bg">
    <div>
        <h1> The easiest way to start your business in Hong Kong </h1>
        <p> We are the incorporation experts — it's fast, easy, affordable and done right. </p>
    </div>
    <form class="main2_form_bg" action="POST">
        <input type="text" placeholder="Proposed company name"/>
        <button type="button"> Check Avalability </button>
    </form>
    <div>
        <p class="ofert_p_bg"> Packages from HK$490 + fees paid to the government   Typically takes 5 - 10 mins to complete. </p>
    </div>
</section>
</template>

<script>
export default {
    
}
</script>

<style scoped>
    .main2_bg{
        display: block;
        width:40%;
    }
    h1{
        font-family: 'Playfair Display', serif; 
        font-size:48px;
        opacity: 0.8;
    }
    p{
        font-family: 'Muli', sans-serif;
        color:gray;
        font-size:1em;
    }
    .ofert_p_bg{
        font-size:11px;
    }
    .main2_form_bg{
        display:flex;
        width:100%;
    }
    .main2_form_bg button{
        font-family: 'Muli', sans-serif;
        border:none;
        cursor: pointer;
        padding-left: 41px;
        padding-top:1px;
        width: 195px;
        height: 50px;
        border-radius: 25px;
        font-size: 16px;
        line-height: 50px;
        text-align: left;
        position: absolute;
        display: flex;
        align-self: center;
        right:70px;
        background:#ff4a5a;
        color:white;
    }
    .main2_form_bg input{
        font-family: 'Muli', sans-serif;
        outline:none;
        opacity: 0.5;
        border:1px solid gray;
        padding: 0 25px;
        width: calc(100% - 140px);
        height: 50px;
        border-radius: 25px;
        box-sizing: border-box;
    }
</style>