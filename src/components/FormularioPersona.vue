<template>
  <div id="formulario-persona">
    <form @submit.prevent="enviarFormulario">
      <div class="container">
        <div class="row">
          <div class="col-md-4">
            <div class="form-group">
              <label>Nombre</label>
              <input v-model="persona.nombre" type="text" class="form-control" />
            </div>
          </div>
          <div class="col-md-4">
            <div class="form-group">
              <label>Apellido</label>
              <input v-model="persona.apellido" type="text" class="form-control" />
            </div>
          </div>
          <div class="col-md-4">
            <div class="form-group">
              <label>Email</label>
              <input v-model="persona.email" type="email" class="form-control" />
            </div>
          </div>
        </div>
        <div class="row">
          <div class="col-md-4">
            <div class="form-group">
              <button class="btn btn-primary">Añadir persona</button>
            </div>
          </div>
        </div>
      </div>
    </form>
  </div>
</template>

<script>
  export default {
  name: 'formulario-persona',
  data() {
    return {
      persona: {
        nombre: '',
        persona: '',
        apellido: '',
      },
    }
  },
  methods: {
    enviarFormulario() {
      console.log('Funciona!');
    },
  },
}
</script>

<style scoped>
  form {
    margin-bottom: 2rem;
  }
</style>