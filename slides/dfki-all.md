---
title: DFKI
---

<div style="float: left; width:35%; top:10px;">
  <img src="https://eric-rietzke.github.io/P_SPELL/img/dfki-germany2.png" />
</div>

<div style="float: right; width:60%;">
  Deutsches Forschungszentrum für Künstliche Intelligenz gGmbH <br><br>
  <v-card class="mx-auto" :theme="theme">
    <v-list density="compact">
        <v-list-item :active=true title="Europas größte Forschungseinrichtung für KI"/>
        <v-list-item prepend-icon="mdi-account-group" title="800 hochqualifizierte Forscher und Mitarbeiter"/>
        <v-list-item prepend-icon="mdi-account-group-outline" title="560 studentische Mitarbeiter"/>
        <v-list-item prepend-icon="mdi-earth" title="aus 65 Nationen"/>
        <v-list-item prepend-icon="mdi-vector-intersection" title="25 Forschungsbereiche / 9 Kompetenzzentren"/>
        <v-list-item prepend-icon="mdi-file-document-outline" title="über 400 laufende Forschungsprojekte"/>
        <v-list-item :active=true title="Außenstelle Trier (seit 2020)"/>
        <v-list-item prepend-icon="mdi-brain" title="Erfahrungsbasierte Lernende Systeme (Prof. Bergmann)"/>
        <v-list-item prepend-icon="mdi-head-cog-outline" title="Kognitive Sozialsimulation (Prof. Timm)"/>
    </v-list>
</v-card>
</div>

<script setup>
import { ref } from "vue";
const theme = ref("dark");
const options = {
  attributes: true
}
function callback(mutationList, observer) {
  mutationList.forEach(function(mutation) {
    if (mutation.type === 'attributes' && mutation.attributeName === 'class') {
      const mode = document.getElementsByTagName("html")[0].classList[0];
      theme.value = mode;
    }
  })
}
const observer = new MutationObserver(callback)
observer.observe(document.getElementsByTagName("html")[0], options)
theme.value = document.getElementsByTagName("html")[0].classList[0] || "dark"
</script>

