<!DOCTYPE html>
 <html lang="en">
 
 <head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>digital clack</title>
 </head>
 
 <body>
     <!-- <span id="hours"> 00</span>:<span id="minutes"> 00</span>:<span id="seconds"> 00</span>;
     <script>
         var seconds = 60;
         var minutes = 0;
         var hours = 0;
         var timerhandler = setinterval(changetime, 1000);
 
         function changetime() {
             document.getElementById("seconds").innerHTML = string(seconds);
 
             document.getElementById("minutes").innerHTML = string(minutes);
 
             document.getElementById("hours").innerHTML = string(hours);
 
             seconds--;
             if (seconds == 0) {
                 seconds = 60;
                 minutes++;
             }
             if (minutes == 60) {
                 minutes = 0;
                 hours++;
             }
             if (hours == 24) {
                 seconds = 60;
                 minutes = 0;
                 hours = 0;
             }
         } -->
     <p>A Script to Show Digital Clock</p>
 
     <button onclick="myTimer()">Show Clock</button>
 
     <p>Your Clock: <span id="clock"></span></p>
     <script>
         function myTimer() {
 
             let myVar = setInterval(myTimer, 2000);
             let showClock = new Date();
 
             document.getElementById("clock").innerHTML = showClock.toLocaleTimeString();
 
         }
     </script>
 </body>
 
 </html>
