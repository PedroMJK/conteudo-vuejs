<template>
    <TheHeader v-if="showHeader" /> 
    <div class="box">

        <h1 class="h1-content">AULA 02</h1>
        <br>
        <div v-show="showName">
            Nome: {{ firstName }} <br>
            Sobrenome:{{ lastName }}
        </div>
        
          <div v-if="elementOfNature === 'water' ">The Water</div>
          <div v-else-if="elementOfNature === 'fire' ">The Fire</div>
          <div v-else-if="elementOfNature === 'wind' ">The Wind</div>
          <div v-else>The Earth</div>

    </div>
    
    
</template>

<script>
export default {

}
</script>

<style>

.box{
    background: #42b883;
    border-radius: 20px;
    box-shadow: 10px 5px 5px black;
    padding-bottom: 20px;
}

</style>