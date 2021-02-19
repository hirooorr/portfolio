<template>
  <div id="home">
    <Header />
    <img class="back" src="../assets/back.png" >
    <div class="home">
      <div class="content">
        <p>nemuTimez</p>
      </div>
    </div>
  </div>
</template>

<script>
import Header from '../components/Header'
export default {
  components: {
    Header
  }
};
</script>

<style scoped>
.back {
  width: 100%;
}
.content p {
  font-size: 60px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
</style>
