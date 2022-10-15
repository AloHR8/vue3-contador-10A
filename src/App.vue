<script>
    export default{
        data: () => ({
            contador : 500,
        }),
        methods: {
            saludar(){
                console.log("Hola 10A | @")
            },
            incrementar() {
                this.contador++;
            },
            decrementar(){
                this.contador--;
            },
            resetear(){
                this.contador = 10;
            }
        }
    };
</script>

<template>
    <div class="navbar">
        <a href="#"><i class="fa fa-fw fa-search"></i> Alondra Hernandez Reyes </a> 
        <a href="#"><i class="fa fa-fw fa-envelope"></i></a> 
        <a href="#"><i class="fa fa-fw fa-user"></i> 10 A DGS </a>
    </div>
    <br>
    
    
    <div class="container">
        <img src="./assets/logo.svg" alt="logo VUE" width="125">
        <small>
        <h1>Hola Desde VUE.JS 3</h1>
    </small>
    <hr>
    <h2>Contador {{contador }}</h2>
    <button @click="incrementar()">+1</button>
    <button @click="decrementar()">-1</button>
    <button @click="resetear()">Reset</button>
</div>
</template>

<style scoped>
    .navbar {
  width: 100%;
  background-color: #666;
  overflow: auto;
}

.navbar a {
  float: left;
  padding: 12px;
  color: white;
  text-decoration: none;
  font-size: 17px;
}
    .container{
        text-align: center;
    }
    small{
        color: #666;
    }
    h1{
        font-weight: bolder;
    }
    h2{
        font-size: 2.5rem;
    }
    button{
        cursor: pointer;
        font-size: 1.5rem;
        margin: 0px 8px;
    }
</style>