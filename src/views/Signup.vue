<template>
  <div id="signup">
    <Header />
    <img class="back" src="../assets/back.png" >
    <div class="form">
      <input placeholder="Name" type="name">
      <input placeholder="Email" type="email">
      <input placeholder="Password" type="password">
      <button @click="auth">signup</button>
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
.form {
  height: 230px;
  padding: 20px;
  background-color: whitesmoke;
  border-radius: 15px;
  text-align: center;
  position: absolute;
  top: 50%;
  left:50%;
  transform: translate(-50%, -50%);
}
input {
  margin: 25px;
  border-radius: 4px;
  display: flex;
  flex-direction: column;
  border-color:whitesmoke;
}
input:hover {
  letter-spacing: 5px;
  transition: .2s;
}
button {
  border-radius: 5px;
  padding: 5px 15px;
  color: black;
  cursor: pointer;
  border: 0;
}
button:hover {
  letter-spacing: 5px;
  transition: .2s;
}
</style>
