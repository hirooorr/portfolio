<template>
  <div id="home">
    <Header />
    <img class="back" src="../assets/back.png" >
    <div class="home">
      <p>nemuTimez</p>
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
.home p {
  color: white;
  font-size: 60px;
  position: absolute;
  top: 55%;
  left: 50%;
  transform: translate( -55%, -50%);
}
</style>
