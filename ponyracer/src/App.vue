<template>
  <main class="container" style="margin-top: 70px">
    <h1>Ponyracer</h1>
    <h2>Welcome {{ user.name }}</h2>
    <Races></Races>
    <!-- <h2>{{ numberOfUsers }} users</h2> -->
  </main>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue';
import Races from './Races.vue';

export default defineComponent({
  name: 'App',

  components: {
    Races
  },
  setup() {
    /* const numberOfUsers = ref(146);
    setTimeout(() => (numberOfUsers.value = 147), 3000);
    return { numberOfUsers }; */
    const user = ref({
      id: 1,
      name: 'Jessica'
    });
    return { user }; 
  }
});
</script>

<style></style>
