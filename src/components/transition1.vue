<template>
    <div>
        <div v-if="yes" class="div1">vue1</div>
        <div v-if="yes" class="div1">vue2</div>
        <div v-if="yes" class="div1">vue3</div>

    </div>
</template>

<script>
export default {
    data(){
        return{
            yes: 'true';
        }
    }
}
</script>


<style lang="scss">
    .div1{
        width:100px;
        height:100px;
        background:red;
    }
</style>