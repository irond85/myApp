<template>
  <ion-page>
    <ion-content :fullscreen="true">
      <div id="padre">
        <div id="redondeo">
        </div>
        <div id="card">
          <ion-card id="login">
            <div class="inputs">
              <InputComponent :label="`USUARIO`" :placeholder="`USUARIO`" :iconL="`USUARIO`" />
              <InputComponent :label="`USUARIO`" :placeholder="`USUARIO`" :tipo="`password`" :iconL="`USUARIO`" />
            </div>
            <div class="button">
              <ButtonComponent :title="`INGRESAR`" />
            </div>
            <div class="button">
              <ion-button fill="clear">
                ¡REGISTRATE!
              </ion-button>
            </div>
            <ion-button>
                ¡REGISTRATE!
              </ion-button>
          </ion-card>
        </div>
      </div>
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import InputComponent from './../components/InputComponent.vue';
import ButtonComponent from './../components/ButtonComponent.vue';
import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar } from '@ionic/vue';

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

#padre {
  position: relative;
  height: 100%;
}

#redondeo {
  position: relative;
  z-index: 50;
  height: 80%;
  border-radius: 0% 0% 50% 50%;
  background: linear-gradient(#7FE5F0, #7FE5F0);
  display: flex;
  justify-content: center;
  align-items: center;
}

#card {
  position: absolute;
  z-index: 100;
  top: 25%;
  left: 4%;
  width: 100%;
  height: 100%;
}

ion-card {
  --background: #fff;
  width: 85%;
  height: 60%;
  padding: 30% 2%;
}

#container a {
  text-decoration: none;
}

.button {
  display: flex;
  justify-content: center;
}
</style>
