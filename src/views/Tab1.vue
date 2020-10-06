<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Tab 1</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content>
      <ion-item @click="() => $router.push('tab1/child')" detail>To Child</ion-item>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
  import {IonPage, IonItem, IonHeader, IonToolbar, IonTitle, IonContent} from '@ionic/vue';
  import {defineComponent} from 'vue';

  export default defineComponent({
    name: 'Tab1',
    components: {IonHeader, IonToolbar, IonTitle, IonContent, IonPage, IonItem}
  })
</script>
