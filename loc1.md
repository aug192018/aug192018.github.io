---
title: Heart of Centretown
CustomReturn: true
---

<div style="text-align:center">
  <p align="center">
    Downtown, in a planter on Kent between Albert and Slater.
  </p>
</div>

<div style="text-align:center">
<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d4710.025622366988!2d-75.70739115844336!3d45.41744562661835!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zNDXCsDI1JzAzLjMiTiA3NcKwNDInMTQuMiJX!5e0!3m2!1sen!2sca!4v1535345331391" width="300" height="300" frameborder="0" style="border:0" allowfullscreen></iframe>
</div>
  
<hr>
  
<br>
<div style="text-align:center">
  <p align="center">
    <h2>When you've arrived...</h2>
    Here we are! What's the name of the store across the street?
  </p>
</div>
<br>

<div style="text-align:center">
  <form id="FirstQ" onSubmit="dogs(); return false;">
    <input type="text" id="answer" name="user_name" />
    <input type="button" value="Check" onclick="dogs(); return false;" />
  </form>
</div>

<div style="text-align:center">
  <p id="demo"></p>
</div>

<div id="FirstAnswer" style="display: none; text-align:center">
  <hr>
  <br>
  <h2>A closer look</h2>
  <img id="imgFirstAnswer" src="none.jpg" height="534" width="300">
  <br>
</div>  

<div id="SecondAnswer" style="display: none; text-align:center">
  <hr>
  <br>
  <h2>The last step</h2>
  Find your gentleman friend and say to him the magical phrase:
  <b>
  <p id="DecodedMessage" style="color:rgb(43, 255, 195)"></p>
  </b>
  <br>
</div>  

<script src = "/7571101397556063/htools.js"></script>

<script>
  loadLib("/7571101397556063/htools.js");
  function dogs() {
      var text = document.getElementById("FirstQ").elements[0].value;
      var HashResult = lazyHash(text);
      //text = text + "<br>" + HashResult;

      setCookie("FirstAnswerCookie", text, 365)
      //document.getElementById("demo").innerHTML = text;

    if (HashResult == 229439158001674) 
    {
      document.getElementById("demo").innerHTML = "Success!";
      document.getElementById("imgFirstAnswer").src = f("img.jpg");
      document.getElementById("FirstAnswer").style.display = "block";
    }
    else 
    {
      document.getElementById("demo").innerHTML = "Try again :( <br> (Your last try was: \"" + text + "\")";
      document.getElementById("FirstAnswer").style.display = "none";
    }
  }

  function f(ta) {
   //Cheater!!
   //alert("/" + parseInt((lazyHash("1510129177")-lazyHash("crumblies") + 31)/1000000000) + "/" + ta);
   return "/" + parseInt((lazyHash("1510129177")-lazyHash("crumblies") + 31)/1000000000) + "/" + ta;
  } 

  function lazyHash(InString) {
      var hash = 5381;
      for(var i = 0; i < InString.length; i++)
      {
         hash = hash*33 + InString.charCodeAt(i);
      }
      return hash;
  }

  function setCookie(cname, cvalue, exdays) {
      var d = new Date();
      d.setTime(d.getTime() + (exdays * 24 * 60 * 60 * 1000));
      var expires = "expires="+d.toUTCString();
      document.cookie = cname + "=" + cvalue + ";" + expires + ";path=/";
  }

  function getCookie(cname) {
      var name = cname + "=";
      var ca = document.cookie.split(';');
      for(var i = 0; i < ca.length; i++) {
          var c = ca[i];
          while (c.charAt(0) == ' ') {
              c = c.substring(1);
          }
          if (c.indexOf(name) == 0) {
              return c.substring(name.length, c.length);
          }
      }
      return "";
  }

  function getParameterByName(name) {
      name = name.replace(/[\[]/, "\\[").replace(/[\]]/, "\\]");
      var regex = new RegExp("[\\?&]" + name + "=([^&#]*)"),
          results = regex.exec(location.search);
      return results === null ? "" : decodeURIComponent(results[1].replace(/\+/g, " "));
  }

  /////////////
  /////////////
  alert(A_Decode("HNtbgbhnwsujump4hnqawsgbp4wxwshnecqap4azjmhn!!"));


  var PreviousFirstAnswer = getCookie("FirstAnswerCookie");
  if (lazyHash(PreviousFirstAnswer) == 229439158001674)
  {
    document.getElementById("FirstQ").elements[0].value = PreviousFirstAnswer;
    document.getElementById("demo").innerHTML = "Success!";
    document.getElementById("imgFirstAnswer").src = f("img.jpg");
    document.getElementById("FirstAnswer").style.display = "block";
  }

  var SecondAnswer = getParameterByName("sa")
  if (lazyHash(SecondAnswer) == 7571710509952919)
  {
    document.getElementById("FirstQ").elements[0].value = PreviousFirstAnswer;
    document.getElementById("demo").innerHTML = "Success!";
    document.getElementById("imgFirstAnswer").src = f("img.jpg");
    document.getElementById("FirstAnswer").style.display = "block";

    document.getElementById("SecondAnswer").style.display = "block";
    document.getElementById("DecodedMessage").innerHTML = A_Decode("HNtbgbhnwsujump4hnqawsgbp4wxwshnecqap4azjmhn!!");
  }

</script>
