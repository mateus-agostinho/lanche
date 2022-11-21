<template>
  <div id="app">
    <header>
      <a href="#" class="logo"><i class="fas fa-utensils"></i>Food</a>

      <nav class="navbar">
        <a href="#home">Home </a>
        <a href="#Special">Especial </a>
        <a href="#popular">Popular </a>
      </nav>

    </header>


   
  </div>
</template>

<script>

</script>

<style>
*{
  font-family: 'Nunito', sans-serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  outline: none;
  border: none;
  text-decoration: none;
  text-transform: capitalize;
  transition: all .2s linear;
}
body{
  background: #f7f7f7 ;
}
header{
  position: fixed;
  top: 0; 
  left: 0; 
  right: 0;
  z-index: 1000;
  display: flex;
  align-items: center;
  justify-content: space-between;
  background: #fff;
  padding: 2rem 9%;
  box-shadow:0 .5rem 1rem rgb(0,0,0, .1) ;
}
header .logo{
  font-size: 2.5rem;
  font-weight: bolder;
  color: #666;
}
header .logo i{
  padding-right: .5rem;
  color: rgb(134, 7, 7);
}

</style>
