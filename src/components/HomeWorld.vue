<template>
    <div>
    <h1>This is our Home</h1>
     <h2>how are you</h2> 
    <h3> {{data}} </h3>
    <h4> {{ msg }} </h4>
    <button v-on:mousehover="hello('Spam')">Call Hello Function</button>
    <h5 v-if="show">Testing Conditional rendering</h5>
    <h5 v-else >Testing Conditional else rendering</h5>
    <button v-on:click="display"> Toggle Element</button> 
    </div>
</template>  

<script>

export default {
    name: 'HomeWorld',
    props : {
        data: String,
        msg : String 
    },
    // methods : {
    //     hello(data){
    //         alert(data);
    //     },
        data(){
            return {show:false}
        },
        methods :{
            display(){
                this.show=!this.show
            }
        }
    
}
</script>
