<template>
  <div>soy footer, la operacion es {{ operacion }}</div>
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
      return operacion;
    },
  },
};

</script>

<style></style>
