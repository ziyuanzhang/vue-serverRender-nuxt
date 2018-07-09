<template>
    <div>
        <h1>asyncData:</h1>
        <p>name:{{info.name}}</p>
        <p>age:{{info.age}}</p>
    </div>
</template>

<script>
import  axios from "axios";
export default {
    data(){
        return{
            titel:"titel"
        }
    },
   /*  asyncData(){
        return axios.get("https://api.myjson.com/bins/shkum")
        .then((res)=>{
            return {info:res.data}
            })
        .catch((err)=>{
            return err;
        })
    } */
    async asyncData(){
        let {data} = await axios.get("https://api.myjson.com/bins/shkum");
        return { info:data}
    }
}
</script>
