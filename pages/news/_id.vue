<template>
    <div>
        <h1>new details page</h1>
        <p>{{$route.params.id}}</p>
    </div>
</template>
<script>
export default {
    validate ({ params }){
        return /^\d+$/.test(params.id)
    }
    
}
</script>

