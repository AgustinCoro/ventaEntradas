/* eslint-disable */
<template>
  <div>
    <v-row class="mt-5">
      <v-col cols="4">
        <v-img
          lazy-src="../assets/ratablanca-sde.jpg"
          max-height="560"
          max-width="800"
          src="../assets/ratablanca-sde.jpg"
          contain
          class="ma-2"
        ></v-img>
        <v-card
          variant="outlined"
          elevation="22"
          class="mt-20, ml-5"
          color="yellow"
          v-on="descargarICS"
        >
          <v-card-title>Sincronizar Calendario</v-card-title>

          <v-card-text>
            <!-- <v-icon color="primary">mdi-map-marker</v-icon> -->
            Descarga el archivo ICS, luego importa el evento a tu propio
            calendario utilizando programas como Google Calendar, Microsoft
            Outlook o Apple Calendar
          </v-card-text>
          <v-card-actions class="d-flex justify-center">
            <v-btn icon>
              <v-icon color="blue" size="24">mdi-facebook</v-icon>
            </v-btn>
            <v-spacer></v-spacer>
            <v-btn icon>
              <v-icon color="lightblue" size="24">mdi-twitter</v-icon>
            </v-btn>
            <v-spacer></v-spacer>
            <v-btn icon>
              <v-icon color="green" size="24">mdi-whatsapp</v-icon>
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col cols="8">
        <v-card variant="outlined" elevation="22" class="mr-3">
          <v-card-title>RATA BLANCA EN SANTIAGO</v-card-title>

          <v-card-text>
            <v-icon color="primary">mdi-map-marker</v-icon>
            Cayococo SDE Autopista Santiago La Banda La Banda, Santiago del
            Estero.
          </v-card-text>
          <v-card-text>
            <v-icon color="primary">mdi-calendar-month</v-icon>
            Apertura de Puertas: 20:00hs
          </v-card-text>
          <v-card-text>
            <v-icon color="primary">mdi-ticket-outline</v-icon>
            Entradas Online Desde: ARS 6000
          </v-card-text>
          <v-card-text>
            <v-icon color="primary">mdi-credit-card-settings-outline</v-icon>
            Formas de Pago: Tarjeta de D??bito y Cr??dito
          </v-card-text>
          <v-card-text>
            <v-icon color="primary">mdi-exclamation-thick</v-icon>
            NO COMPRES TU ENTRADA EN REVENTA. Todos los asistentes al evento
            ser??n controlados con su DNI al ingresar.
          </v-card-text>
          <v-card-actions>
            <v-autocomplete
              v-model="value"
              :items="items"
              dense
              filled
              label="Horarios"
            ></v-autocomplete>
            <v-spacer></v-spacer>
            <v-btn fab big dark color="primary" class="mb-5">
              <v-icon>mdi-cash</v-icon>
            </v-btn>
          </v-card-actions>
        </v-card>

        <div class="d-flex justify-center; mt-10">
          LA IC??NICA BANDA SE PRESENTA EN SANTIAGO DEL ESTERO EN EL COMPLEJO
          CAYOCOCO EL JUEVES 16 DE MARZO LA BANDA M??S IMPORTANTE DEL HARD ROCK Y
          HEAVY METAL, LLEGA A SANTIAGO DEL ESTERO , LLEVANDO TODO SU REPERTORIO
          DE CL??SICOS Y GRANDES ??XITOS EN ESTA GIRA NACIONAL QUE COMIENZA EL 2
          DE MARZO EN VARIAS CIUDADES DEL PA??S. Rata Blanca se la considera como
          una de las m??s importantes e influyentes del hard rock y heavy en
          espa??ol, aunque durante su carrera tambi??n ha incorporado pesados
          riffs con estructuras mel??dicas y arm??nicas de la m??sica cl??sica. Con
          los a??os han clasificados en distintos subg??neros, sin embargo, la
          banda se considera simplemente "rock met??lico". El grupo se lanza al
          estrellato en la d??cada del '90, destacando como una de las bandas
          argentinas m??s populares de todos los tiempos. Tres de sus ??lbumes han
          sido incluidos entre los mejores 250 del rock iberoamericano. Su
          carrera parece impulsarse a los m??s altos niveles cuando en 1990
          publican su segundo disco, Magos, Espadas y Rosas, con m??s de 5
          millones de copias vendidas hasta la actualidad, logrando varias
          distinciones, y que le ha valido el comienzo de una larga hegemon??a en
          el contexto internacional, estableciendo firmemente su reputaci??n como
          banda en vivo. Muchos de sus temas han logrado un alcance de
          popularidad hasta entonces inimaginable para el rock pesado. Ostentan
          durante su trayectoria 6 discos de oro y 1 de platino, haci??ndolos la
          banda del g??nero m??s exitosa de su pa??s, como as?? tambi??n una de las
          m??s reconocidas internacionalmente. La qu??mica se basa en el
          virtuosismo de Walter Giardino y la poderosa voz de Adri??n Barilari.
          Desde sus comienzos, la banda ha sufrido varios cambios en su
          formaci??n, siendo Walter Giardino el ??nico miembro original que
          permanece hasta hoy. Su alineaci??n actual est?? formada por Walter
          Giardino (guitarra), Adri??n Barilari (voz), Fernando Scarcella
          (bater??a), Pablo Motyczak (bajo) y Danilo Moschen (teclados). SHOW:
          RATA BLANCA EN SANTIAGO DEL ESTERO FECHA: JUEVES 16 DE MARZO HORA:
          21:00 HS VENUE: CAYOCOCO DIRECCION: AUTOPISTA SANTIAGO LA BANDA
        </div>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  name: "EjemploView",
  data: () => ({
    items: ["16-03-2023, 21:00 HS"],
    values: ["foo", "bar"],
    value: null,
  }),

  methods: {
    descargarICS() {
      console.log("Presiono el evento de descargarICS");
    },
  },
};
</script>

<style></style>
