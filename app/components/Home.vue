<template>
  <Page>
    <ActionBar>
      <Label text="BABY" class="font-bold text-lg" />
      <ActionItem
        ios.systemIcon="9" ios.position="left"
        android.systemIcon="ic_menu_share" android.position="actionBar" />
    </ActionBar>

    

    <TabView androidTabsPosition="bottom">
        <TabViewItem title="First">
          <Dashboard></Dashboard>
        </TabViewItem>
        <TabViewItem title="Second">
          <Label text="Second Tab Content" textAlignment="center" verticalAlignment="center" />
        </TabViewItem>
        <TabViewItem title="Third">
          <Label text="Third Tab Content" textAlignment="center" verticalAlignment="center" />
        </TabViewItem>
      </TabView>
  </Page>
</template>

<script lang="ts">
import { AbsoluteLayout, FlexboxLayout, GridLayout, Image, ScrollView, StackLayout, TabView } from '@nativescript/core';
import Vue from 'nativescript-vue';

import Dashboard from '@/components/Dashboard.vue'

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
  components: {
    Dashboard
  }
});
</script>

<style scoped>

</style>
