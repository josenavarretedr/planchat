<template>
  <div>
    <!-- Crear un formulario básico con dos input un correo y una contraseña y un botón -->
    <h1>Formulario bASE</h1>
    <form>
      <input type="email" placeholder="Email" /> <br />
      <input type="password" placeholder="Password" />
      <button>Registro</button>
    </form>
  </div>
</template>

<script>
import router from "@/router";

export default {
  name: "SignForm",

  data() {
    return {
      email: "",
      password: "",
    };
  },

  setup() {
    const onSubmit = async (e) => {
      e.preventDefault();
      const { email, password } = e.target.elements;
      try {
        await register(email.value, password.value);
        router.push("/");
      } catch (error) {
        alert(error.message);
      }
    };

    return {
      onSubmit,
    };
  },
};
</script>
