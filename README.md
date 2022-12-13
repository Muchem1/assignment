# assignment
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!--Leaflet css file-->
    <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.1/dist/leaflet.css"
     integrity="sha256-sA+zWATbFveLLNqWO2gtiw3HL/lh1giY/Inf1BJ0z14="
     crossorigin=""/>
     <!--Leaflet javascript file-->
     <script src="https://unpkg.com/leaflet@1.9.1/dist/leaflet.js"
     integrity="sha256-NDI0K41gVbWqfkkaHj15IzU7PtMoelkzyKp8TOaFQ3s="
     crossorigin=""></script> 
    <title>Westlands</title>
</head>
<body>
  
    <h1 style = "color:rgb(81, 13, 88)" >WEB MAPPING</h1>  
    <h2 style = "color:rgb(81, 13, 88)" >WEB PAGE</h2>
    
    <div id="map", style="height: 300px"></div>
<script>
    var map = L.map('map').setView([ -1.25615, 36.805373], 13);
    L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
    maxZoom: 19,
    attribution: '@ OpenStreetMap'
}).addTo(map);

var marker = L.marker([ -1.25615, 36.805373]).addTo(map);
marker.bindPopup("<b>THE COOPER IVY</b><br>MUNCHIES HAVEN.").openPopup();

function onMapClick(e) {
    alert("You clicked the map at " + e.latlng);
}

map.on('click', onMapClick);
</script>

</body>
<footer>
    <h1 style = "color:rgb(44, 44, 141)"></h1>
</footer>
</html>
Footer
© 2022 GitHub, Inc.
