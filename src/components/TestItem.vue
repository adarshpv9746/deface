<template>
    <div>
        <h1>Az033 {{data}}</h1>
        <a href="adzvue.netlify.app">{{msg}}</a>
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
