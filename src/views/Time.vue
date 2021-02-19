<template>
  <div id="time">
    <Header2 />
    <div class="time">
        <div class="content">
            <div class="timecard">
                <p>明日の起床時間は</p>
                <select class="timeReserve" v-model="selected">
                    <option disabled value="">時間選択</option>
                    <option v-for="time in times"
                        :value="time.res"
                        :key="time.id">
                    {{ time.reserve }}
                    </option>
                </select>
                <p>です</p>
                <span>Selected: {{ selected }}</span>
            </div> 
            <div @click="edit">
                <button @click="decide">set</button> 
            </div> 
        </div>
        <Tool />
    </div>
  </div>
</template>

<script>
import Tool from '../components/tool'
import Header2 from '../components/Header2'
export default {
  data() {
    return {
        selected: '',
        times: [
            { res: "0:00" },
            { res: "0:00" },
            { res: "0:00" },
            { res: "0:00" },
            { res: "0:00" },
            { res: "0:00" },
            { res: "0:00" },
            { res: "0:00" },
            { res: "0:00" },
            { res: "0:00" },
            { res: "0:00" },
        ],
    };
  },
  components: {
    Header2,
    Tool
  },
  methods: {
      decide: function() {
          alert("起床時間を設定しました");
      }
  }
}
</script>

<style>
#time {
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
.timeReserve {
    cursor: pointer;
    display: block;
    margin: 0 auto;
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