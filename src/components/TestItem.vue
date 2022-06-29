<template>
    <div>
        <!-- <h1>Az033 {{data}}</h1>
        <a href="adzvue.netlify.app">{{msg}}</a> -->
        <h3>
        <button class="button button1" v-on:click="button('green')">Green</button>
        <button class="button button2" v-on:click="button('blue')">Blue</button>
        </h3>
    </div>
</template>
<script>
export default {
    name: "TestItem",
    props:{
        data:String,
        msg:String
    }, methods:{
        button(a){
                alert(a+' button clicked')
        }
    }
}
</script>
<style>
.button {
  border-radius: 100px;
  border: none;
  color: white;
  padding: 15px 60px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 20px;
  cursor: pointer;
}
.button1 {background-color: #4CAF50;} /* Green */
.button2 {background-color: #008CBA;} /* Blue */
</style>
