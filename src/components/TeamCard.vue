<template>
  <div>
  
      <div class="card text-white bg-dark">
        <div class="d-flex justify-content-center p-2">
          <img :src="member.img" alt="Imagen integrante" class="img-fluid">
        </div>
        <div class="card-body">
          <h4 class="card-title">{{member.nombre}}</h4>
          <p class="card-text">
           {{member.codigo}}. {{member.info}}
          </p>
          <p class="card-text"><span>Rol: </span> {{member.rol}}</p>
        </div>
        <div class="card-footer">
          <small class="text-muted">last updated </small>
        </div>
      </div>
    </div>
 
</template>

<script>
export default {
  name: "TeamCard",
  props: {
      'member' : Object
  }
};
</script>

<style scoped>
</style>
