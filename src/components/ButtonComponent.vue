<template>
    <ion-button>{{ title }}</ion-button>
</template>
  
<script lang="ts">
import { IonButton } from '@ionic/vue';
import { defineComponent } from 'vue';

export default defineComponent({
    components: { IonButton },
    props: ['title']
});
</script>
  
<style scoped>
ion-button {
    --background: #193046;
    --color-activated: white;
    --background-hover: #193046;
    --background-activated: #193046;
    --background-focused: #193046;

    --color: #7FE5F0;
    --border-radius: 10px;
    --border-color: #193046;

    font-weight: bold;
}
</style>