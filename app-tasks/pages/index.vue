<template>
  <div>
    <center>
      <h1>Bienvenidos a la app de tareas</h1>
      <v-spacer></v-spacer>
      <v-card
        class="mx-auto"
        max-width="344"
        title="Registro de Usuario"
      >
        <v-container>
          <v-text-field
            v-model="first"
            color="primary"
            label="Primer Nombre"
            variant="underlined"
          ></v-text-field>

          <v-text-field
            v-model="last"
            color="primary"
            label="Apellido"
            variant="underlined"
          ></v-text-field>

          <v-text-field
            v-model="email"
            color="primary"
            label="Email"
            variant="underlined"
          ></v-text-field>

          <v-text-field
            v-model="password"
            color="primary"
            label="Contraseña"
            placeholder="Enter your password"
            variant="underlined"
          ></v-text-field>

          <v-checkbox
            v-model="terms"
            color="secondary"
            label="Acepto los términos y condiciones"
          ></v-checkbox>
          <a href="/iniciar"> Ya tengo cuenta </a>
        </v-container>

        <v-divider></v-divider>
        
        <v-card-actions>
          <v-spacer></v-spacer>
        
          <v-btn color="success">
            <a href="/tareas"> Ingresar</a>
            <v-icon icon="mdi-chevron-right" end></v-icon>
          </v-btn>
        </v-card-actions>
      </v-card>
    </center>

  </div>
</template>
<script>
definePageMeta({
  layout: "blank",
});
</script>