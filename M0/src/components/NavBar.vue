<template>
    <div class="navbar__items">
      <a href="/login"><button>Login</button></a>
      <a href="/about">Services</a>
      <a href="/about">About</a>
      <a href="/about">Home</a>
      <div class="logo">
       <img src="../assets/images/guitar.jpg" alt="">
       <p>My company</p>
      </div>
    </div>
</template>

<style scoped>
.navbar__items {
  background-color: black;
  overflow: hidden;
}

.navbar__items a {
    float: right;
    color: white;
    text-align: center;
    padding: 14px 16px;
    text-decoration: none;
    font-size: 15px;
}

.navbar__items button {
    background-color: grey;
    color: white;
}
.logo img{
 float: left;
 padding: 0px 10px 0px 10px;
 height: 30px;
 width: 30px;
 border-radius: 50%;
}
.logo p {
    color: white;
    text-align: left;
   padding: 5px;
    font-size: 0.8rem;
    
}

</style>
