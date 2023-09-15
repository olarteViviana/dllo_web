<template>
    <div class="ma-5">
        <v-card
            class="mx-auto"
            width="400"
            prepend-icon="mdi-home"
        >
            <template v-slot:title>
                Iniciar Sesión
            </template>

            <v-card-text>
                <v-sheet max-width="300" class="mx-auto">
                    <v-form validate-on="submit lazy" @submit.prevent="submit">
                        <v-icon :icon="`mdiSvg:${mdiAccount}`"></v-icon>
                        <v-text-field
                            v-model="userName"
                            :rules="rules"
                            label="User name"
                        ></v-text-field>

                        <v-icon icon="fa:fas fa-lock"></v-icon>
                        <v-text-field
                            v-model="password"
                            :rules="rules"
                            label="Contraseña"
                        ></v-text-field>

                        <v-btn
                            :loading="loading"
                            type="submit"
                            block
                            class="mt-2"
                            text="Ingresar"
                        ></v-btn>
                    </v-form>
                </v-sheet>
            </v-card-text>
        </v-card>
    </div>
  </template>