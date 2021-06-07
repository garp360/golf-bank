<template>
  <ion-page>
    <ion-content :fullscreen="true">
      <FormContainer />
    </ion-content>
  </ion-page>
</template>

<script>
import { IonPage, IonContent } from '@ionic/vue';
import FormContainer from '@/components/FormContainer.vue';

export default  {
  name: 'Money',
  components: { FormContainer, IonContent, IonPage }
}
</script>