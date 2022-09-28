# Vorstellung
Dr. Eric Rietzke

<div style="position: absolute; height: 90%; width: 70%; right: 2%; top: 5%; font-size: 90%;">

<v-timeline :theme="theme">
<v-timeline-item>Studium der Informatik <br>Hochschule Trier</v-timeline-item>
<v-timeline-item class="text-right">20 Jahre Praxiserfahrung <br>Gründer, Unternehmer, Vorstand</v-timeline-item>
<v-timeline-item>Promotion Universität Trier <br>Forschungsschwerpunkt: <br>wissensintensive Prozesse</v-timeline-item>
<v-timeline-item class="text-right">
    Senior Researcher / DFKI <br>
    FB Smarte Daten & Wissensdienste<br>
    Erfahrungsbasierte Lernende Systeme<br>
    Projektleiter SPELL
</v-timeline-item>
</v-timeline>
</div>

<div style="position: absolute; left: 5%; top: 30%;">
<img src="./public/img/pic-eric.jpg" style="margin-top:-20px;" class="h-62 rounded shadow" />
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
