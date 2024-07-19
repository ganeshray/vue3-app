<template>
  <div>
   <v-container>
        <v-row justify="center">
          <v-col cols="12" md="8">
          <v-btn @click="increment" class="ma-2">Increment</v-btn> 
           <v-chip
              class="ma-2"
              color="black"
              text-color="white"
              label
              pill
            >
              {{ count }}
            </v-chip>
          </v-col>
        </v-row>
      </v-container>
  </div>
</template>

<script>
import { mapActions, mapGetters } from 'vuex';

export default {
  name: 'HomePage',

   computed: {
    ...mapGetters(['count']),
  },
  methods: {
    ...mapActions(['increment']),
  }
};
</script>

<style scoped>
h1 {
  color: #42b983;
}
</style>