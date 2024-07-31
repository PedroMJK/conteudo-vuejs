<template>
        <!-- 08 - LIGACÕES DE DADOS BIDIRECIONAL (DIRETIVA V-MODEL) -->

        <div class="box">
            <h1 class="h1-content">AULA 06</h1>
            <br>

            <div>
              One-way data binding <br>
              Two-way data binding <br>
              v-model -> formulários
            </div>
            <br>
        
            <div>
              <label>Name</label> <br>
              <input 
                  v-model="name"
                  type="text"> <br>
                  {{ name }}
        
                  <br><br>
        
            <div>
                <label>Character</label> <br>
                <select v-model="character">
                  <option value="">Escolha</option>
                  <option value="goku">Goku</option>
                  <option value="naruto">Naruto</option>
                  <option value="vegeta">Vegeta</option>
                </select> <br>
                {{ character }}
            </div>
        
            <br><br>
        
            <div>
              <label>Newsletter</label> <br>
              <input 
                  v-model="newsletter"
                  type="radio"
                  value="Yes">Sim
              <input 
                  v-model="newsletter"
                  type="radio"
                  value="No">Não
            </div> <br>
        
            {{ newsletter }}
        
              <br><br>
        
              <label>Contrato</label> <br>
              <input 
                  v-model="contract"
                  type="checkbox"
                  value="">Aceita nossos termos...
                  <br>
                  {{ contract }}
        
                  <br><br>
                  
                  <label>Cores que você mais gosta</label> <br>
                  <input 
                      v-model="colors"
                      type="checkbox"
                      value="Verde"> Verde <br>
                  <input 
                      v-model="colors"
                      type="checkbox"
                      value="Vermelho"> Amarelo <br>
        
                      {{ colors }}
            </div>
        
          </div>    

</template>

<script>
export default {

    data() {
        return{
          name: 'Pedro',
          character: '',
          newsletter: '',
          contract: false,
          colors: [],
        }
    }
}

</script>

<style>


</style>