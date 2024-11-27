<template>
  <Page>
    <ActionBar>
      <Label text="BABY" class="font-bold text-lg" />
    </ActionBar>

    <ListView height="100%" for="item in flicks">
      <v-template>
        <Label :text="item.title" />
      </v-template>
    </ListView>
  </Page>
</template>

<script lang="ts">
import Vue from 'nativescript-vue';

export default Vue.extend({
  computed: {
    message() {
      return 'Blank {N}-Vue app';
    },
  },

  methods: {
    logMessage() {
      console.log('You have tapped the message!');
    },
  },
});
</script>

<style>
/* .info {
    font-size: 20;
  } */
</style>
