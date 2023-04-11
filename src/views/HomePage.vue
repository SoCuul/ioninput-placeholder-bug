<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-title>Blank</ion-title>
      </ion-toolbar>
    </ion-header>

    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Blank</ion-title>
        </ion-toolbar>
      </ion-header>

      <ion-row class="ion-justify-content-center">

        <ion-col size="3" class="pn-col flex-centered">
          <ion-input id="pn-1" maxlength="3" type="text" value="number" inputmode="numeric" placeholder="123" class="text-centered pn-input" onkeypress="return /[0-9]/i.test(event.key)"></ion-input>
        </ion-col>
        <ion-col size="1" class="pn-col flex-centered">
          <h1 class="pn-separator">-</h1>
        </ion-col>
        <ion-col size="3" class="pn-col flex-centered">
          <ion-input id="pn-2" maxlength="3" type="text" value="number" inputmode="numeric" placeholder="456" class="text-centered pn-input" onkeypress="return /[0-9]/i.test(event.key)"></ion-input>
        </ion-col>
        <ion-col size="1" class="pn-col flex-centered">
          <h1 class="pn-separator">-</h1>
        </ion-col>
        <ion-col size="3" class="pn-col flex-centered">
          <ion-input id="pn-3" maxlength="4" type="text" value="number" inputmode="numeric" placeholder="7890" class="text-centered pn-input" onkeypress="return /[0-9]/i.test(event.key)"></ion-input>
        </ion-col>

      </ion-row>
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar, IonRow, IonCol, IonInput } from '@ionic/vue';
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

.text-centered {
    text-align: center;
}
.flex-centered {
    display: flex;
    justify-content: center;
}

.label-wrap {
    padding-right: 0.625rem;
    white-space: normal;
}

.pn-label-margins {
    margin-top: 0;
    
    margin-right: -1rem;
    margin-left: -1rem;
}

.pn-col {
    padding-top: 0;
}

.pn-input {
    border: 0.125rem solid var(--ion-color-light-tint);
    border-radius: .28125em
}
.pn-input.ios {
    --padding-start: 8px !important;
}

.pn-separator {
    margin-top: 0.625rem;
}

ion-item {
    --background: none;
}
</style>
