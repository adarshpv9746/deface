<template>
    <div>
        <h1>Sorry we are currently developing..</h1>
        <h2>{{data}}{{msg}}</h2>
    </div>
</template>
<script>
export default {
    name: "TestItem",
    props:{
        data:String,
        msg:String
    }
}
</script>
