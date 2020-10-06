<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-buttons>
          <ion-back-button default-href="tab1" />
        </ion-buttons>

        <ion-title>Child</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content>
      Route: {{ route.params.name }}
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
  import {IonPage, IonButtons, IonBackButton, IonHeader, IonToolbar, IonTitle, IonContent} from '@ionic/vue';
  import {defineComponent} from 'vue';
  import {useRoute} from "vue-router";

  export default defineComponent({
    name: 'ChildTab',
    components: {IonHeader, IonToolbar, IonTitle, IonContent, IonPage, IonButtons, IonBackButton},
    setup() {
      return {
        route: useRoute(),
      }
    },
  })
</script>
