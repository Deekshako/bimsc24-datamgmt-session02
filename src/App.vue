<script setup>
import { ref, computed } from "vue";

let name = ref("This is a signup form for a serious website");

// For the text input
const inputText = ref('');

 // Change the type of input to password or text
 function Toggle() {
            let temp = document.getElementById("typepass");
             
            if (temp.type === "password") {
                temp.type = "text";
            }
            else {
                temp.type = "password";
            }
        }

</script>


<template>
 <div id="navbar" class="container">  
        <div id="title">{{name}}</div>
        </div>

    <div id="flex">

    <div id="sidebar" class="container">

    <input v-model="inputText" placeholder="Type your thoughts here">
    <br>
    <input v-model="color" placeholder="Your least favourite color">
    <br>
    <input v-model="emailid" placeholder="Email id">
    <br>
    <input type="password" placeholder="password" id="typepass">
    <br>
    <button class="GFG" 
    onclick="window.location.href ='https://www.youtube.com/watch?v=dQw4w9WgXcQ&ab_channel=RickAstley'"> Click Submit
    </button> 

    </div>

        <div id="main" class="container"> Text input </div>
    </div>

</template>

<style scoped>
html{
    background-color: grey; 
    color: white;
    font-family: Arial, Helvetica, sans-serif;
}

body{
    margin:0;
}

div{
    /* put the borders in the inside of container */
    box-sizing: border-box;
}

#navbar{
    height: 50px;
    border-color: red;
}

#flex{
    display: flex;
    height: calc(100vh - 50px);
}

#sidebar_1{
    width:30%;
    border-color: blue;
}

#main{
    width:40%;
    border-color: green;
}

#sidebar_2{
    width:30%;
    border-color: yellow;
}

#title{
    width: 70%;
    float:left;
}

.container{
    border-style: dotted;
    border-width: 1px;
}

</style>
