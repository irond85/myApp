<template>
    <ion-item>
        <ion-input :label="`${label}`" label-placement="floating" fill="outline" :placeholder="`${placeholder}`"
            :type="`${tipo}`">
            <ion-icon slot="start" :icon="iconL" aria-hidden="true"></ion-icon>
        </ion-input>
    </ion-item>
</template>
  
<script lang="ts">
import { IonItem, IonList, IonInput, IonIcon } from '@ionic/vue';
import { defineComponent } from 'vue';
import { mail } from 'ionicons/icons';

export default defineComponent({
    components: { IonList, IonItem, IonInput, IonIcon },
    props: ['label', 'placeholder', 'tipo', 'iconL'],
    setup() { return { mail } },
});
</script>

<style scoped>
ion-item {
  margin-bottom: 30px;
}
</style>