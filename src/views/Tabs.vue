<template>
  <ion-page>
      <ion-header>
      <ion-toolbar>
        <ion-title>GOLF BANK</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-tabs>
      <ion-tab-bar slot="bottom">
        <ion-tab-button tab="tab1" href="/tabs/pheasants">
          <ion-icon :icon="people" />
          <ion-label>Pheasants</ion-label>
        </ion-tab-button>

        <ion-tab-button tab="tab2" href="/tabs/money">
          <ion-icon :icon="cash" />
          <ion-label>Money</ion-label>
        </ion-tab-button>

        <ion-tab-button tab="tab3" href="/tabs/games">
          <ion-icon :icon="golf" />
          <ion-label>Games</ion-label>
        </ion-tab-button>
      </ion-tab-bar>
    </ion-tabs>
  </ion-page>
</template>

<script>
import {
  IonTabBar,
  IonTabButton,
  IonTabs,
  IonLabel,
  IonIcon,
  IonPage,
  IonHeader, IonToolbar, IonTitle
} from "@ionic/vue";
import { people, cash, golf } from "ionicons/icons";

export default {
  name: "Tabs",
  components: { IonLabel, IonHeader, IonToolbar, IonTitle, IonTabs, IonTabBar, IonTabButton, IonIcon, IonPage },
  setup() {
    return {
      people,
      cash,
      golf,
    };
  },
};
</script>