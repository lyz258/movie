<template>
    <div >
        <ul class="footer">
            <li>电影</li>
            <li>音乐</li>
            <li>书籍</li>
            <li>图书</li>
        </ul>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
    .footer{
        width: 100%;
        height: 50px;
        background-color: rgb(33, 150, 243);
        position: fixed;
        bottom: 0;
        display: flex;
    }
    .footer li{
       flex-grow: 1;
       text-align: center;
       line-height: 50px;
       color: azure; 
    }
</style>
