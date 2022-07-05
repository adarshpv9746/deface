<template>
    <div>
        <!-- <h1>Az033 {{data}}</h1>
        <a href="adzvue.netlify.app">{{msg}}</a> -->
        <h1 class="center">
        <img v-if="show" alt="Vue logo" src="https://upload.wikimedia.org/wikipedia/commons/c/c7/Loading_2.gif">
        <img v-if="!walk" alt="Vue logo" src="https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/1abfa455389655.59822ff82373e.gif" >
        <img v-if="!fly" alt="Vue logo" src="https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/4029a055389655.59822ff823c19.gif" >
        <img v-if="!drive" alt="Vue logo" src="https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/0f7cda43377507.57ecc15d6620f.gif" >
        </h1>
        <h2 class="testitem">
        <button class="button button1" v-if="fly" v-on:click="button('fly')">Fly</button>
        <button class="button button1" v-if="!fly" v-on:click="button('fly')">fly</button>
        <button class="button button2" v-if="drive" v-on:click="button('drive')">Drive</button>
        <button class="button button2" v-if="!drive" v-on:click="button('drive')">drive</button>
        <button class="button button3" v-if="walk" v-on:click="button('walk')">Walk</button>
        <button class="button button3" v-if="!walk" v-on:click="button('walk')">walk</button>

        </h2>
    </div>
</template>
<script>
export default {
    name: "TestItem",
    props:{
        data:String,
        msg:String
    },data(){
        return{show:true,fly:true,drive:true,walk:true}
        },
        methods:{
        button(a){
                // alert(' button clicked')
                if(a=='fly'){
                    this.fly=!this.fly;
                    this.walk=true;
                    this.drive=true;
                    
                }
                else if(a=='drive'){
                    this.drive=!this.drive;
                    this.walk=true;
                    this.fly=true;
                    
                }
                else{
                    this.walk=!this.walk;
                    this.fly=true;
                    this.drive=true;
                    
                }
                this.show=false;

                
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
.button3 {background-color: #494f51;}
.center {
  position: absolute;
  top:  50%;
  left: 50%;
  transform: translate(-50%,-50%);
}
.testitem{
  position: relative;
  top:  505px;
  left: 50%;
  transform: translate(-50%,-50%);
}
</style>
