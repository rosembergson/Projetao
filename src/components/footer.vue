<template>
    <div class="footer_bg">
      <div class="footer_bg--bg">
        <div class="first_footer_bg">
            <h1> Want to set up your business today? </h1>
            <p>See if your proposed company is available for incorporation or <span>contact us</span></p>
        </div>
        <form action="POST"class="form_bg">
            <input type="text" placeholder="search">
            <button type="button">Check Avalability</button>
        </form>
        <li> Packages from HK$490 + fees paid to the government   Typically takes 5 - 10 mins to complete.</li>
        <div class="list_bottom_bg">
            <ul>
                <li>TERMS AND CONDITIONSPRIVACY </li>
                <li>- POLICYCOOKIE </li>
                <li>- POLICY</li>
            </ul>
            <p></p>
        </div>
      </div> 
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
    .footer_bg{
        width:100%;
        height:500px;
        display:flex;
        justify-content: center;
        text-align: center;
        background: #ff4a5a; 
        font-family: 'Muli', sans-serif;
        color:#2e3038;
    }
    .footer_bg--bg{
        width:100%;
    }
    .first_footer_bg{
        width:30%;
        text-align:center;
    }
    .footer_bg h1{
        font-family: 'Playfair Display', serif; 
        color:white;
        font-size:40px;
    }
    .footer_bg p{
        font-size:16px;
    }

    .form_bg{
        display: flex;
        justify-content: flex-end;
        padding:10px 20px;
        background:transparent;  
        width:50%;
        text-align:center;
    }
    .form_bg input{
        position: relative;
        outline:none;
        width:50%;
        border:none;
        background:rgba(0,0,0,0.3);
        padding:21px 30px;
        border-radius:30px;
        color:rgba(255, 255, 255, 2);
    }
    .footer_bg--bg input::placeholder{
        color: rgba(255, 255, 255, 0.3);

    }

    .footer_bg--bg button{
        display:flex;
        align-self: flex-end;
        padding: 21px 30px;
        border:none;
        outline: none;
        cursor: pointer;
        border-radius:30px;
        position: absolute;
        box-sizing: border-box;
        background: #2e3038;
        color:white;
    }

    /* lista footer */

    .list_bottom_bg{
        display:flex;
        justify-content: space-between;
        margin-bottom:0;
    }

    .list_bottom_bg ul{
        display:flex;
        list-style: none;
        align-content:unset;
        flex-direction: row;
    }
</style>