<template>
  <div class="tool">
    <div class="type">
      <img class="share" @click="$router.push('/share')" src="../assets/home.png" alt="">
      <img class="time" @click="$router.push('/time')" src="../assets/time.png" alt="">
      <img class="profile" @click="$router.push('/profile')" src="../assets/profile.png" alt="">
      <img class="exit" src="../assets/exit.png" alt="">
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.tool {
  position: absolute;
  bottom: 0;
  left: 10%;
  right: 10%;
  mix-blend-mode: multiply;
  position: fixed;
  cursor: pointer;
  z-index: 10;
}
.type {
  height: 150px;
  display: flex;
  flex-direction: row;
  justify-content: center;
}
.type img {
  margin: 0 30px;
}
</style>