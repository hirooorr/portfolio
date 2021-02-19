<template>
    <div class="header flex">
        <div class="left">
            <img src="../assets/logo.png" class="logo" />
        </div>
        <div class="right flex">
            <p @click="$router.push('/signup')">signup</p>
            <p @click="$router.push('/login')">login</p>
        </div>
    </div>
  
</template>

<script>
export default {

}
</script>

<style scoped>
.header {
    z-index: 10;
    height: 50px;
}
.logo {
    padding: 5px;
    height: 40px;
}
.header {
    background-color: white;
}
.right {
    align-items: center;
}
.right p {
    margin-right: 20px;
    color: black;
    cursor: pointer;
}
.flex {
    display: flex;
    justify-content: space-between;
}
</style>