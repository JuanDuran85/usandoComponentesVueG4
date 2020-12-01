<template>
<section class="container">
    <div v-for="(item, index) in dataUser" :key="index">
      <div>
      <img :src="item.src" :alt="item.nombre" class="img-fluid mt-4">
      </div>
      <div>
          <div id="resultados" class="resultados row mx-auto text-center">
            <p>{{item.nombre}}</p>
          </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Lista',
  props: {
    dataUser: {
      type: Array,
      required: true,
      default(){
        return [
          {nombre: 'no tiene', src: 'no tiene'}
        ]
      }
    }
  },

  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  img {
    border-radius: 50%;
    margin-left: 20px;
    width: 200px;
    
  }
</style>
