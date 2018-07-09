<template>
    <div>
        <nav class="news-nav">
            <ul>
                <li>
                    <nuxt-link to="/news/123">news123</nuxt-link>
                </li>
                <li>
                    <nuxt-link :to="{name:'news-id',params:{id:456}}">news456</nuxt-link>
                </li>
                <li>
                    <nuxt-link to="/news/aaa">newaaa</nuxt-link>
                </li>
            </ul>
        </nav>
        <p>i am news</p>
        <p>newsId:{{$route.params.newsId}}</p>
        <p>data:{{newID}}</p>
    </div>
</template>
<script>
export default {
    data(){
        return{
            newID:this.$route.params.newsId
        }
    },
    head(){
        return{
            title:"news",
            meta:[
                {hid:"description",name:"news",content:"this is news"}
            ]
        }
    },
    transition:'test'
}
</script>
<style lang="scss" scoped>
.news-nav>ul{
    width: 150px;
    background-color:#ccc;
    li{
       border: 1px solid #000;
       a{
           display: inline-block;
           width: 100%;
       }
    }
    
}
</style>


