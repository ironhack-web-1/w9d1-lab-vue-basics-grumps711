<template>
  <div>aqui navbar y el resultado de esta operacion es {{ operacionDelNavBar }}</div>
</template>

<script>
export default {
  data() {
    return {
      operation: 3 * 6,
    };
  },
  computed:{
    operacionDelNavBar(){
      return this.operation;
    }
  }
};
</script>

<style></style>