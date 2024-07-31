<template>

<div class="box">
    <h1 class="h1-content">AULA 05</h1>
    <br>

    <div>   
        <h1 :class="{'title': true, 'title-home': isHome }">
          Curso Vue 3
        </h1>
      </div>
    
          <!--Segunda forma -->  
      <div>
        <p :class="pClass">
          Lorem ipsum dolor sit amet consectetur 
          adipisicing elit. Earum, quod quibusdam. 
          Doloremque cum veritatis laudantium provident nemo!
          Quibusdam voluptate eveniet, accusamus dolor quisquam 
          maiores eum voluptatibus ut vitae obcaecati fugiat!
        </p>
        
        <p :style="styleClass">
          Lorem ipsum dolor sit amet consectetur 
          adipisicing elit. Earum, quod quibusdam. 
          Doloremque cum veritatis laudantium provident nemo!
          Quibusdam voluptate eveniet, accusamus dolor quisquam 
          maiores eum voluptatibus ut vitae obcaecati fugiat!
        </p>
    
      </div>
    
      <div>
          <img 
           v-bind:src="imgSrc"
           :alt="imgAlt"
           class="img">
      </div>
    
      <div>
    
        <div
            v-for="(obj, index) in todos" 
            v-bind:key="obj.id"
            class="todos-item"
        >
            {{ index }} - {{ obj.title }}
        </div>
    
      </div>   
    
</div>

   
</template>

<script>
export default {
      isHome: true,
      pClass: ['text', 'text-home' ],
      styleClass: {color: 'aqua', backgroundColor: 'black' },

      imgSrc: 'https://via.placeholder.com/600/92c952',
      imgAlt: 'Foto do v-bind',

}
</script>

<style>


.title{
    font-size: 30px;
    color: red;
  } 
  
  .title-home{
    font-size: 60px;
    color: greenyellow;
  }
  
  .text {
    font-size: 25px;
    color: purple;
  }
  
  .text-home{
    font-size: 20px;
    color: rgb(47, 168, 255);
  }
  
  .img {
    border: 2px solid;
    border-radius: 50px;
    height: 80px;
  }
</style>
