<template>
  <div class="container">
    <div id="yaMap" style="height: 400px; background-color: yellow"></div>
    <div id="googleMaps" style="height: 400px; background-color: yellow"></div>
  </div>
</template>

<script>
import ymaps from "ymaps";
/* import 'google-maps' as gmaps; */

/* gmaps.load(function(google) {
  new google.maps.Map(el, options);
});
 */
ymaps
  .load()
  .then(maps => {
    const map = new maps.Map("yaMap", {
      center: [-8.369326, 115.166023],
      zoom: 7
    });
  })
  .catch(error => console.log("Failed to load Yandex Maps", error));

/* gmaps.createClient({
    key: 'AIzaSyBFlJvRnzuIJo_Et-c48xss9hcUeS_eUZk'
}) */

export default {
  name: "test-maps"
};
</script>
