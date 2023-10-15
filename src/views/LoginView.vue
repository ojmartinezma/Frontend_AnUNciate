<template>
  <div class="login">
    <LoginPage></LoginPage>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import LoginPage from "@/components/LoginPage.vue"; // @ is an alias to /src

export default defineComponent({
  name: "LoginView",
  components: {
    LoginPage,
  },
});
</script>
