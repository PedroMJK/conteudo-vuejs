<!--        EVENTOS  -->

<template>

    <div class="box"> 
        <h1 class="h1-content">AULA 07</h1>
        <br>
    
        <div>
            <button v-on:click="onClick()">
                Enviar
            </button>
        </div> <br>
    
        <div @mouseover="onMouseOver()">
            Mouse Over
        </div>
    
    </div>
    </template>
    
    <script>
        export default {
            name: 'Component09',
            
            methods: {      // Onde ficará as funções.
                onClick() {
                  console.log("Clicou");
                },
    
                onMouseOver() {
                    console.log("Mouse Over")
                }
            }
        } 
    
    </script>

