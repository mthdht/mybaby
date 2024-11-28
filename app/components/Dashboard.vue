<template>
    <ScrollView>
        <StackLayout class="bg-red-100 p-4 space-y-8">
        <!-- Conteneur pour l'image et les informations superposées -->
        <AbsoluteLayout rows="auto" columns="*" class="relative w-full h-[800px]">
            <!-- Image du bébé -->
            <Image src="~/assets/baby-photo.jpg" class="absolute w-full h-full rounded-lg object-cover bg-yellow-300" />
            <!-- Overlay -->
            <FlexboxLayout top="400" class="w-full" alignItems="center">
            <Label text="Alexendria" class="text-2xl font-bold pl-6" flexGrow="1"/>
            <Label text="6 mois" class="text-lg font-semibold px-4" />
            <Label text="7.5 kg" class="text-lg font-semibold pr-6" />
            </FlexboxLayout>
        </AbsoluteLayout>
        
        <GridLayout class="bg-blue-300 h-96">
            <label text="ok"></label>
        </GridLayout>
        </StackLayout>
    </ScrollView>   
</template>
  
<script lang="ts">
import { AbsoluteLayout, FlexboxLayout, GridLayout, Image, ScrollView, StackLayout } from '@nativescript/core';
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

<style scoped>

</style>
  