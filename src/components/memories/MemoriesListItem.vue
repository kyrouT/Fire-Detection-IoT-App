<template>
    <ion-item  
        :router-link="`/sensors/${memory.id}`">
          <ion-thumbnail slot="start">
            <ion-img :src="memory.img" :alt="memory.title"></ion-img>
          </ion-thumbnail>
          <ion-label>
            {{memory.title}}
          </ion-label>
        </ion-item>
</template>

<script>
import {IonItem, IonThumbnail,IonImg,IonLabel} from "@ionic/vue"

export default {
    props: ["memory"],
    components: {
        IonItem,
        IonThumbnail,
        IonImg,
        IonLabel
    }  
}
</script>