
<template>
 
    <div class="wrapper">
      <NavBar />
      <SearchBar />
      <TeacherImage />
     
    </div>
 

  
</template>
<script>
import SearchBar from "./components/SearchBar.vue"
import NavBar from "./components/NavBar.vue"
import TeacherImage from "./components/TeacherImage.vue"
export default {
   name:"app",
   components: {
    SearchBar,
    NavBar,
    TeacherImage
   }
    

}
</script>

<style>



/* @media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
} */
</style>
