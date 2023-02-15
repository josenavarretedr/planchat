<template>
  <div>
    <!-- Crear un formulario básico con dos input un correo y una contraseña y un botón -->
    <h1>Register</h1>
    <!-- <RegisterForm /> -->
    <SignForm></SignForm>
  </div>
</template>

<script>
import RegisterForm from "../components/RegisterLogin/RegisterForm.vue";
import SignForm from "../components/RegisterLogin/SignForm.vue";

export default {
  name: "Register",
  components: {
    // RegisterForm,
    SignForm,
  },
  setup() {
    // const { register } = useAuth();
    // const { user } = useUser();
    // const router = useRouter();

    // const onSubmit = async (e) => {
    //   e.preventDefault();
    //   const { email, password } = e.target.elements;
    //   try {
    //     await register(email.value, password.value);
    //     router.push('/');
    //   } catch (error) {
    //     alert(error.message);
    //   }
    // };

    // if (user) {
    //   router.push('/');
    // }

    return {
      // onSubmit,
    };
  },
};
</script>
