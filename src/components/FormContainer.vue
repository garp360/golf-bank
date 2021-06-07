<template>
  <div id="container">
    <ion-button size="large" color="success">WON</ion-button>
    <ion-button size="large" color="dark">LOST</ion-button>
    <div><strong>You Phucking Pheasant</strong><br /><br /></div>
    <!-- <p>Explore <a target="_blank" rel="noopener noreferrer" href="https://ionicframework.com/docs/components">UI Components</a></p> -->
    <ion-item>
      <ion-label>Game</ion-label>
      <ion-select interface="action-sheet" placeholder="Game">
        <ion-select-option value="matchplay1">Match Play</ion-select-option>
        <ion-select-option value="stableford">Stableford</ion-select-option>
        <ion-select-option value="tournament">Tournament</ion-select-option>
      </ion-select>
    </ion-item>
    <div>
      <ion-toolbar>
        <ion-segment value="all">
          <ion-segment-button value="all"> INDIVIDUAL </ion-segment-button>
          <ion-segment-button value="favorites">TEAMS</ion-segment-button>
        </ion-segment>
      </ion-toolbar>
      <ion-item>
        <ion-label>Opponent</ion-label>
        <ion-select
          :interface-options="customActionSheetOptions"
          interface="action-sheet"
          placeholder="Opponent"
        >
          <ion-select-option value="1003">Burke</ion-select-option>
          <ion-select-option value="1005">Dahlenburg</ion-select-option>
          <ion-select-option value="1004">Devine</ion-select-option>
          <ion-select-option value="1006">Friedman</ion-select-option>
          <ion-select-option value="1002">Miller</ion-select-option>
          <ion-select-option value="1001">Murdza</ion-select-option>
          <ion-select-option value="1003">Burke</ion-select-option>
          <ion-select-option value="1005">Dahlenburg</ion-select-option>
          <ion-select-option value="1004">Devine</ion-select-option>
          <ion-select-option value="1006">Friedman</ion-select-option>
          <ion-select-option value="1002">Miller</ion-select-option>
          <ion-select-option value="1001">Murdza</ion-select-option>
          <ion-select-option value="1003">Burke</ion-select-option>
          <ion-select-option value="1005">Dahlenburg</ion-select-option>
          <ion-select-option value="1004">Devine</ion-select-option>
          <ion-select-option value="1006">Friedman</ion-select-option>
          <ion-select-option value="1002">Miller</ion-select-option>
          <ion-select-option value="1001">Murdza</ion-select-option>
          <ion-select-option value="1003">Burke</ion-select-option>
          <ion-select-option value="1005">Dahlenburg</ion-select-option>
          <ion-select-option value="1004">Devine</ion-select-option>
          <ion-select-option value="1006">Friedman</ion-select-option>
          <ion-select-option value="1002">Miller</ion-select-option>
          <ion-select-option value="1001">Murdza</ion-select-option>
        </ion-select>
      </ion-item>
      <ion-item>
        <ion-label>Opponent</ion-label>
        <ion-select
          :interface-options="customActionSheetOptions"
          interface="action-sheet"
          placeholder="Opponent"
        >
          <ion-select-option value="1003">Burke</ion-select-option>
          <ion-select-option value="1005">Dahlenburg</ion-select-option>
          <ion-select-option value="1004">Devine</ion-select-option>
          <ion-select-option value="1006">Friedman</ion-select-option>
          <ion-select-option value="1002">Miller</ion-select-option>
          <ion-select-option value="1001">Murdza</ion-select-option>
          <ion-select-option value="1003">Burke</ion-select-option>
          <ion-select-option value="1005">Dahlenburg</ion-select-option>
          <ion-select-option value="1004">Devine</ion-select-option>
          <ion-select-option value="1006">Friedman</ion-select-option>
          <ion-select-option value="1002">Miller</ion-select-option>
          <ion-select-option value="1001">Murdza</ion-select-option>
          <ion-select-option value="1003">Burke</ion-select-option>
          <ion-select-option value="1005">Dahlenburg</ion-select-option>
          <ion-select-option value="1004">Devine</ion-select-option>
          <ion-select-option value="1006">Friedman</ion-select-option>
          <ion-select-option value="1002">Miller</ion-select-option>
          <ion-select-option value="1001">Murdza</ion-select-option>
          <ion-select-option value="1003">Burke</ion-select-option>
          <ion-select-option value="1005">Dahlenburg</ion-select-option>
          <ion-select-option value="1004">Devine</ion-select-option>
          <ion-select-option value="1006">Friedman</ion-select-option>
          <ion-select-option value="1002">Miller</ion-select-option>
          <ion-select-option value="1001">Murdza</ion-select-option>
        </ion-select>
      </ion-item>
    </div>
  </div>
</template>

<script>
import {
  IonButton,
  IonItem,
  IonLabel,
  IonSelect,
  IonSelectOption,
} from "@ionic/vue";
import { defineComponent } from "vue";

export default defineComponent({
  name: "FormContainer",
  components: { IonButton, IonItem, IonLabel, IonSelect, IonSelectOption },
  props: {
    name: String,
  },
  data: function() {
    return { 
        
    }
  },
  setup() {
    const customActionSheetOptions = {
      header: "Opponents",
    };

    return {
      customActionSheetOptions,
    };
  },
});
</script>

<style scoped>
#container {
  text-align: center;
  position: absolute;
  left: 0;
  right: 0;
  top: 50%;
  transform: translateY(-50%);
}

#container strong {
  font-size: 20px;
  line-height: 26px;
}

#container p {
  font-size: 16px;
  line-height: 22px;
  color: #8c8c8c;
  margin: 0;
}

#container a {
  text-decoration: none;
}
</style>