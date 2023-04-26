<template>
<div class="cards">
    <article class="card"> 
        <img src="../assets/images/keyboard.jpg" alt="Hot air balloons">
        <div class="content">
            <header>Keyboard </header>
            <p>hello</p>
        </div>
            
    </article>
            
     <article class="card"> 
        <img src="../assets/images/keyboard.jpg" alt="Hot air balloons">
        <div class="content">
            <header>Lopsem</header>
            <p>hello</p>
        </div>
    </article>
            
    <article class="card">
        <img src="../assets/images/keyboard.jpg" alt="Hot air balloons">
        <div class="content">
           <header>Lopsem</header>
           <p>hello</p>
        </div>

    </article>
</div>
</template>
<style scoped>
.cards {
    display: grid;
    grid-gap: 10px;
    grid-template-columns: repeat(3, 1fr);
}

.card {
    display: grid;
    padding: 30px 20px 1px 10px;

    grid-template-rows: max-content 60px;
}

.card img {
    object-fit: cover;
    width: 100%;
    height: 100%;
}
.content {
    background-color: gray;
}
.content header {
   padding-left: 10px;
}
.content p {
 padding: 0px 0px 10px 10px;
}

</style>

