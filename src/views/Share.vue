<template>
  <div id="share">
    <Header2 />
        <div v-for="(value, index) in shares" :key="index">
            <div class="message">
                <div class="post">
                    <h1>経過時間：{{ value.time }}分</h1>
                    <p>評価：{{ value.eva }}</p>    
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
            shares: [
                { time: 30, eva: 2},
                { time: 6, eva: 5}
                ]
        }
    },
    components: {
        Header2,
        Tool
    }
}
</script>

<style>
#share {
    height: 1000px;
    background-color: #e7eaee;
}
.message {
    background-color: #ffffff;
    width: 70%;
    margin: auto;
    border-radius: 15px;
}
.post {
}
.post h1,p {
    color: black;
    font-size: 20px;
    text-align: center;
    margin: 30px;
}
</style>