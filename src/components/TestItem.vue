<template>
    <div>
        <h1>Sorry we are currently developing..{{data}}{{msg}}</h1>
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
