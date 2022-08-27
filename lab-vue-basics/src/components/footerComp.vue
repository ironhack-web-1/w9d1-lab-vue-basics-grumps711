<template>
  <div v-if="show">
    <div>soy footer, la operacion es {{ propertyComputed }}</div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      operacion: 2 + 2,
      show: true,
    };
  },
  computed: {
    propertyComputed() {
      return this.operacion;
    },
  },
};
</script>

<style></style>

<!--create a boolean data inside a Vue component, 
and link it to an HTML element that will
only show up in your template if the condition is set to true.-->
