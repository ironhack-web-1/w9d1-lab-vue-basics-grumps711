<template>
  <div>
    aqui navbar y el resultado de esta operacion es {{ operacionDelNavBar }}
  </div>
  <div>
  
   <h3>Titles</h3>
    <ul>
      <li v-for="eso in Items" :key="eso.title">
        {{ eso.title }}
      </li>
    </ul>

     <h3>Descriptions</h3>
    <ul>
      <li v-for="eso in Items" :key="eso.description">
        {{ eso.description }}
      </li>
    </ul>

     <h3>Content</h3>
    <ul>
      <li v-for="eso in Items" :key="eso.content">
        {{ eso.content }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      operation: 3 * 6,
      Items: [
        { title: "Hola" ,
         description: "Brutal" ,
         content: "acción" },
      
        { title: "Pelicula" ,
         description: "Increible" ,
         content: "Terror" },
      
        { title: "Buena" ,
         description: "Espectacular" ,
         content: "Romance" },
      ],
    };
  },

  computed: {
    operacionDelNavBar() {
      return this.operation;
    },
  },
};
</script>

<style></style>
