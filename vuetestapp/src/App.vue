<template>
    <p>Здарова, {{username}}</p>
    <input @change="setUserName" v-bind:value="username"/>
    <button @click="setUserName">SetName</button>
</template>

<script>
export default {
    data(){
        return{
            username:"JabkaScript",
            
        }
        
    },
    methods: {
        setUserName(e){
            this.username = e.target.value;
        }
    }    
}
</script>

<style></style>