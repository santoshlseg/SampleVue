<template>
    <h1>This is our Home</h1>
    <h2>how are you</h2>
    <h3> {{data}} </h3>
    <h4> {{ msg }} </h4>
    <button v-on:mousehover="hello('Spam')">Call Hello Function</button>
</template>  

<script>

export default {
    name: 'HomeWorld',
    props : {
        data: String,
        msg : String 
    },
    methods : {
        hello(data){
            alert(data);
        }
    }
}
</script>
