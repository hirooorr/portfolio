<template>
  <div id="profile">
    <Header2 />
    <div class="profile">
        <div class="content">
            <div class="post">
                <h1>{{ name }}</h1>  
                <p class="text" v-if="active">{{ profile }}</p>
                <input type="text" v-model="profile" v-else >
                <div @click="edit">
                    <button>edit</button> 
                </div> 
            </div> 
        </div>
    </div>
    <Tool />
  </div>
</template>

<script>
import Tool from '../components/tool'
import Header2 from '../components/Header2'
export default {
  data() {
    return {
        active: true,
        name: "hiro",
        profile: "こんにちは、早起きしたいです。よろしくお願いします。"
    };
  },
  components: {
    Header2,
    Tool
}
}
</script>

<style>
#profile {
    background-color: #e7eaee;
    height: 100vh;
}
.content {
    background-color: #ffffff;
    width: 50%;
    margin: auto;
    border-radius: 15px;
    padding: 50px;
}
button {
    color: black;
    display: block;
    margin: 0 0 0 auto;
}
button:hover{
    letter-spacing: 5px;
    transition: .2s;
}
</style>