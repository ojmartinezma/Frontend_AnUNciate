<template>
  <NavBar></NavBar>
  <div class="d-flex justify-content-center">
    <h1>anUNciate</h1>
  </div>
  <div class="d-flex justify-content-center">
    <form>
      <!-- Email input -->
      <MDBInput
        type="email"
        label="Correo electrónico"
        id="form1Email"
        v-model="form1Email"
        wrapperClass="mb-4"
      />
      <!-- Password input -->
      <MDBInput
        type="password"
        label="Contraseña"
        id="form1Password"
        v-model="form1Password"
        wrapperClass="mb-4"
      />
      <!-- 2 column grid layout for inline styling -->
      <MDBRow class="mb-4">
        <MDBCol class="d-flex justify-content-center">
          <!-- Checkbox -->
          <MDBCheckbox
            label="Recuerdame"
            id="form1LoginCheck"
            v-model="form1LoginCheck"
            wrapperClass="mb-3 mb-md-0"
          />
        </MDBCol>
        <MDBCol>
          <!-- Simple link -->
          <a href="#!">Contraseña olvidada?</a>
        </MDBCol>
      </MDBRow>
      <!-- Submit button -->
      <MDBBtn color="primary" block> ingresar </MDBBtn>
    </form>
  </div>
</template>

<script setup lang="ts">
import NavBar from "./NavBar.vue";
import { MDBRow, MDBCol, MDBInput, MDBCheckbox, MDBBtn } from "mdb-vue-ui-kit";
import { ref } from "vue";

const form1Email = ref("");
const form1Password = ref("");
const form1LoginCheck = ref(true);
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
