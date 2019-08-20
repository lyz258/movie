<template>
    <div>
        <common-header></common-header>
        <router-view/>
        <common-footer></common-footer>
    </div>
</template>

<script>
import CommonHeader from '../common/Header'
import CommonFooter from '../common/Footer'
export default {
    name:'Movie',
    components:{
        CommonHeader,
        CommonFooter
    },
   
}
</script>

<style>

</style>
