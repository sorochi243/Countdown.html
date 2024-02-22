<html>
<head>
<style>
/* Add some style to the timer */
#timer {
  color: black;
  font-size: 30px;
  text-align: center;
  background-color: pink;
  padding: 10px;
  margin: 10px;
}

/* Add some style to the button */
#button {
  color: white;
  font-size: 20px;
  text-align: center;
  background-color: blue;
  padding: 10px;
  margin: 10px;
  border: none;
  cursor: pointer;
}
</style>
<script>
// Set the date and time of the giveaway
var giveaway = new Date("Mar 31, 2024 23:59:59").getTime();

// Update the timer every second
var x = setInterval(function() {

  // Get the current date and time
  var now = new Date().getTime();
    
  // Find the difference between now and the giveaway
  var difference = giveaway - now;
    
  // Calculate the days, hours, minutes and seconds
  var days = Math.floor(difference / (1000 * 60 * 60 * 24));
  var hours = Math.floor((difference % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  var minutes = Math.floor((difference % (1000 * 60 * 60)) / (1000 * 60));
  var seconds = Math.floor((difference % (1000 * 60)) / 1000);
    
  // Display the timer in the element with id="timer"
  document.getElementById("timer").innerHTML = days + "d " + hours + "h "
  + minutes + "m " + seconds + "s ";
    
  // If the countdown is over, display some text and disable the button
  if (difference < 0) {
    clearInterval(x);
    document.getElementById("timer").innerHTML = days + "d " + hours + "h "
  + minutes + "m " + seconds + "s ";
    document.getElementById("button").innerHTML = "CURRENT ENTRY"
    document.getElementById("button").disabled = true;
  }
}, 1000);



</script>
</head>
<body></body>

<img src="C:\Users\User\OneDrive\Desktop\download.jpg " alt="iPhone" width="200" height="250">
<img src="C:\Users\User\OneDrive\Desktop\download.jpg " alt="iPhone" width="200" height="250">
<img src="C:\Users\User\OneDrive\Desktop\download.jpg " alt="iPhone" width="200" height="250">
<h1>OLD iPhone Giveaway</h1>
<p1>We are giving away a brand new iPhone 13 to one lucky winner!</p1>


<p> THE GIVEAWAY ENDS ON THE 31ST OF MARCH 2024</p>

<p>The winner will be announced on Dec 31, 2024 at midnight.</p>




<p>Good luck SHA!</p>

<!-- Display the timer -->
<div id="timer"></div>


</body>
</html>
