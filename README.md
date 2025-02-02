<!DOCTYPE HTML>
<html>
<head>
<title>Creality K1 Filament Filter V2</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>

q {
  position: absolute;
  top: 50%;
  -ms-transform: translateY(-50%);
  transform: translateY(-50%);
  
  left: 50%;
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
}

p {
  position: absolute;
  top: 56%;
  -ms-transform: translateY(-50%);
  transform: translateY(-50%);
  
  left: 50%;
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  
  text-align: center;
  font-size: 30px;
  color: white;
  font-family: courier new;
  
  padding-top: 10px;
}

body {
  background-color: black;
}

.countdown {
  padding-top: 5%;
}

</style>
</head>
<body>

<div>
  <q>
    <a href="https://www.tindie.com/products/TinyPinapple"><img src="https://github.com/justcallmekoko/ESP32Marauder/raw/master/pictures/marauder3L.jpg?raw=true" alt="3D Wiev">
  </q>
</div>

<div>
  <p class="countdown" id="demo"></p>

  <script>
// Set the date we're counting down to
var countDownDate = new Date("sep 1, 2025 12:00:00").getTime();

// Update the count down every 1 second
var x = setInterval(function() {

  // Get today's date and time
  var now = new Date().getTime();
    
  // Find the distance between now and the count down date
  var distance = countDownDate - now;
    
  // Time calculations for days, hours, minutes and seconds
  var days = Math.floor(distance / (1000 * 60 * 60 * 24));
  var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
  var seconds = Math.floor((distance % (1000 * 60)) / 1000);
    
  // Output the result in an element with id="demo"
  document.getElementById("demo").innerHTML = days + "d " + hours + "h "
  + minutes + "m " + seconds + "s ";
  
  document.title = days + "d " + hours + "h "
  + minutes + "m " + seconds + "s ";
    
  // If the count down is over, write some text 
  if (distance < 0) {
    clearInterval(x);
    document.getElementById("demo").innerHTML = "EXPIRED";
  }
}, 1000);
  </script>
</div>

</body>
</html>
