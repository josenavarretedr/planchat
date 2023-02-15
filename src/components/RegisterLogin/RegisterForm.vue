<template>
  <div>
    <!-- Crear un formulario básico con dos input un correo y una contraseña y un botón -->
    <h1>Register</h1>
    <form>
      <input type="email" placeholder="Email" /> <br />
      <input type="password" placeholder="Password" />
      <button>Register</button>
    </form>
  </div>
</template>

<script>
export default {
  name: "RegisterForm",
};
</script>
