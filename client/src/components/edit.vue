<template>
  <div class="container-fluid p-5">
    <div class="row">
      <div class="col-2 align-self-center">
        Nombre
      </div>
      <div class="col-10 p-1">
        <input id="nombre" type="text" v-model="bebida.nombre" name="nombre" placeholder="Nombre" class="form-control">
      </div>
    </div>
    <div class="row">
      <div class="col-2 align-self-center">
        Marca
      </div>
      <div class="col-10 p-1">
        <input id="marca" type="text" v-model="bebida.marca" name="marca" placeholder="Marca" class="form-control">
      </div>
    </div>
    <div class="row">
      <div class="col-2 align-self-center">
        Carbonatada
      </div>
      <div class="col-10 p-1">
        <input type="checkbox" name="carbonatada" v-model="bebida.carbonatada">
      </div>
    </div>
    <div class="row float-right pt-4">
      <button id="cancelar" @click="$router.go(-1)" class="btn btn-danger lg-btn">Cancelar</button>
      <button id="guardar" @click="editar" class="btn btn-primary lg-btn">Editar</button>
    </div>
  </div>
</template>

<script src="./edit.js"></script>
