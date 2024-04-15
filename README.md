<!DOCTYPE html>
<html>
<head>
       <meta name="viewpost" content="width=device-width, initial-scale+1.0">
       <title>Coming soon page - Aayush</title>  
       <link href="style.css"  rel="stylesheet"  type="text/css">
 </head>
 <body>
<div class="container">
           <img src="images/logo.png" class="logo=">
           <div class="content">
            <p>Website is under Maintenance</p>
            <h1>We're<span>Launching</span>  soon</h1>
            <div class="launch-time">
            <div>
                  <p id="days">00</p>
                  <span>Days</span>
            </div>
            <div>
                  <p  id="Hours">00</p>
                  <span>Hours</span>
            </div>
            <div>
                  <p  id="Minutes">00</p>
                  <span>Minutes</span>
            </div>
            <div>
                  <p  id="Second">00</p>
                  <span>Second</span>
            </div>
            </div>
            <button type="button">Learn More <img src="images/triangle.png"></button>

           </div>
           <img src="images/rocket.png" class="rocket">
     </div>

<script>
         var CountDownDate = new Date("May 1 ,2024 00:00:00").getTime();
         var x = setInterval(function(){
            var now =new Date().getTime()
            var distance = CountDownDate-now;

            var days = Math.floor(distance / (1000 * 60 * 60 * 24));
            var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
            var seconds = Math.floor((distance % (1000 * 60)) / 1000);

            document.getElementById("days").innerHTML = days;
            document.getElementById("Hours").innerHTML = hours;
            document.getElementById("Minutes").innerHTML = minutes;
            document.getElementById("Second").innerHTML = seconds;



         },1000);

</script>

 </body>
</html>
