<template>
  <div>soy footer, la operacion es {{ propertyComputed }}</div>
</template>

<script>
export default {
  data() {
    return {
      operacion: 2 + 2,
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
