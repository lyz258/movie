<template>
    <div class="header">
        <el-button type="text" class="home">首页</el-button>
        <h2 class="title">Movie</h2>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
    .header{
        width: 100%;
        height: 50px;
        background-color: rgb(33, 150, 243);
        position: fixed;
        top: 0;
        line-height: 50px;
    }
    .home{
        float: left;
        color:azure;
        margin-left: 10px;
    }
    .title{
        position: absolute;
        left: 40%;
        color: azure;
    }
</style>
