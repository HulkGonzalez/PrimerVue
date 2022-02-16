<template>
  <div>
    <div class="container">
      <h1>Tabla de Usuarios</h1>
      <table class="table">
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">Nombre</th>
      <th scope="col">Apellido</th>
      <th scope="col">RUN</th>
      <th scope="col">Nacimiento</th>
      <th scope="col">Edad</th>
    </tr>
  </thead>
  <tbody>
    <tr v-for="usuario in usuarios" :key="usuario">
      <th scope="row">{{usuario.id}}</th>
      <td>{{usuario.nombre}}</td>
      <td>{{usuario.apellido}}</td>
      <td>{{usuario.run}}</td>
      <td>{{usuario.nacimiento}}</td>
      <td>{{usuario.edad}}</td>
    </tr>
  </tbody>
</table>
    </div>
  </div>
</template>

<script>
import "bootstrap/dist/css/bootstrap.min.css"
export default {
  name: 'App',
  data(){
    return{
      usuarios: [{
        id:1,
        nombre:"Cesar",
        apellido: "Gonzalez",
        run: "12.127.952-5",
        nacimiento: "06-12-1978",
        edad: "43",
      },
      {
        id:2,
        nombre:"Felipe",
        apellido: "Gonzalez",
        run: "18.848.636-3",
        nacimiento: "22-11-1992",
        edad: "29",
      },
      {
        id:3,
        nombre:"Jazmin",
        apellido: "Soto",
        run: "16.176.110-9",
        nacimiento: "25-10-1986",
        edad: "36",
      }],
    }
  }
}
</script>

<style>
#app {
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  text-align: center;
  margin-top: 5%;
}
</style>