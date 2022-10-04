<template>
  <navbar />
  <div>aqui la app</div>
  <footerC />

  <button
    class="btn m-1"
    type="button"
    @click="clicked = !clicked"
    :class="[{ clicked: clicked }]"
  >
    Soy el boton que pronto cambiará de color
  </button>
  <form class="form">
    <input v-model="textModel" type="text" placeholder="Name" id="textField" />
    <input v-model="emailModel" type="email" placeholder="email" />
  </form>
  <div>
    <p>Tu nombre es: {{ textModel }}</p>
    <p>Tu email es: {{ emailModel }}</p>
  </div>
  <div>
    <textarea v-model="message"></textarea>

    <p>{{ message }}</p>
    <p>{{ message }}</p>
  </div>
</template>

<script>
import footerC from "./components/footerComp.vue";
import navbar from "./components/navBarComp.vue";

export default {
  components: {
    footerC,
    navbar,
  },
  data() {
    return {
      clicked: false,
      message: null,
      textModel: null,
      emailModel: null,
    };
  },
  methods: {
    debug(event) {
      console.log(event);
    },
  },
  computed: {
    console: () => console,
    window: () => window,
  },
};
</script>

<style scoped>
button {
  margin-top: 50px;
}
#textField {
  margin-top: 50px;
}
.form {
  display: flex;
  flex-direction: column;
  width: 200px;
}
.btn {
  background-color: lightcoral;
  border-radius: 40px;
}
</style>
