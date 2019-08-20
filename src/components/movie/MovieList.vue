<template>
    <ul>
        <li v-for="itme in movieList" :key="itme.id">
            <img :src="itme.big" alt="">
        </li>
    </ul>
</template>

<script>
import Axios from 'axios'
export default {
    data(){
        return{
            movieLists:[],
            movieList:[],
        }
    },
    methods:{
        getmoviList(){
            this.axios.get('http://route.showapi.com/852-2', {
            params: {
                showapi_appid:96965,
                showapi_sign:'3c658057e16e4c46999048d708539a15',
                type:4001,
                page:2,
                itemId:'ed42be1eb076b8e4'
            }
            })
            .then(response=> {
                console.log(response);
                this.movieLists=response.data.showapi_res_body.pagebean.contentlist;
                this.movieList=response.data.showapi_res_body.pagebean.contentlist[6].list;
                console.log(this.movieLists);
                
            })
            .catch(function (error) {
                console.log(error);
            })
            .then(function () {
                // always executed
            });  
        },
        
    },
    mounted(){
        this.getmoviList();
    }
}
</script>

<style>

</style>
