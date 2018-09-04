---
title: Under Wellington
CustomReturn: true
---

<div style="text-align:center">
  <p align="center">
    Along Wellington, well before the bridge to Victoria Island, there's a walking path that takes you down below to the bike lanes. Walking away from downtown, the way down is on your right. If you've made it to the large three-way intersection, you've gone much too far. You should see an underpass under that runs under Wellington St. Below that is another underpass. You're interested in the plaza near the first underpass, immediately below street level.
  </p>
</div>

<div style="text-align:center">
<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2800.52312977945!2d-75.71141150850185!3d45.4189549921601!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zNDXCsDI1JzA4LjIiTiA3NcKwNDInMzYuMyJX!5e0!3m2!1sen!2sca!4v1536028700475" width="300" height="300" frameborder="0" style="border:0" allowfullscreen></iframe>
</div>
  
<hr>
  
<br>
<div style="text-align:center">
  <p align="center">
    <h2>When you've arrived...</h2>
    There's a large sign by the underpass that tells the story of the murals lining the tunnel walls. It gives us a word for 'taking care of oneself'. What is it (without any special accents)? 
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
  <p id="fa_txt"></p>
  <br>
</div>  

<div id="SecondAnswer" style="display: none; text-align:center">
  <hr>
  <br>
  <h2>The last step</h2>
  Find your gentleman friend and say to him the magical phrase:
  <br>
  <b>
  <p id="DecodedMessage" style="color:rgb(43, 215, 215);font-size:22px"></p>
  </b>
  <br>
</div>  

<script src = "/7571101397556063/htools.js"></script>

<script>
  var img_fa  = "IMAG0218.jpg"
  var h_fa    = 3.2273678467801637e+26
  var h_sa    = 8244727662634403000
  
  function dogs() {
      var text = document.getElementById("FirstQ").elements[0].value;
      var HashResult = lazyHash(text);
      //text = text + "<br>" + HashResult;

      setCookie("loc6_FirstAnswerCookie", text, 365)
      //document.getElementById("demo").innerHTML = text;

    if (HashResult == h_fa) 
    {
      document.getElementById("demo").innerHTML = "Success!";
      document.getElementById("imgFirstAnswer").src = f(img_fa);
      document.getElementById("fa_txt").innerHTML = A_Decode("HNqatbp4wxqzfvfvwstbfvp4wwqztgtgp4wxfvtbqzrfgbp4ynazfvp4hnqafvtbtbp4wwtbwsfvrvp4tgwshnhntgtbp4fvtbechnqzujumtgrrp4hnqawsujumgb,,p4azsxsxazgbwshntbp4ynfvazyhp4hnqatbp4gbwsumuj..p4UMwsqqtbp4tbyhp4qzp4tgazazrf!!");
      document.getElementById("FirstAnswer").style.display = "block";
    }
    else if (HashResult == 210726503048)
    {
      alert("Reset!");
      setCookie("loc6_SecondAnswerCookie", "", 365);
    }
    else 
    {
      document.getElementById("demo").innerHTML = "Try again :( <br> (Your last try was: \"" + text + "\")";
      document.getElementById("FirstAnswer").style.display = "none";
      document.getElementById("SecondAnswer").style.display = "none";
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

  var PreviousFirstAnswer = getCookie("loc6_FirstAnswerCookie");
  if (lazyHash(PreviousFirstAnswer) == h_fa)
  {
    document.getElementById("FirstQ").elements[0].value = PreviousFirstAnswer;
    document.getElementById("demo").innerHTML = "Success!";
    document.getElementById("imgFirstAnswer").src = f(img_fa);
    document.getElementById("fa_txt").innerHTML = A_Decode("HNqatbp4wxqzfvfvwstbfvp4wwqztgtgp4wxfvtbqzrfgbp4ynazfvp4hnqafvtbtbp4wwtbwsfvrvp4tgwshnhntgtbp4fvtbechnqzujumtgrrp4hnqawsujumgb,,p4azsxsxazgbwshntbp4ynfvazyhp4hnqatbp4gbwsumuj..p4UMwsqqtbp4tbyhp4qzp4tgazazrf!!");
    document.getElementById("FirstAnswer").style.display = "block";
  }

  var SecondAnswer = getParameterByName("sa")
  var PreviousSecondAnswer = getCookie("loc6_SecondAnswerCookie");
  if (lazyHash(SecondAnswer) == h_sa)
    {setCookie("loc6_SecondAnswerCookie", SecondAnswer, 365); LoadAll();} 
  else if (lazyHash(PreviousSecondAnswer) == h_sa)
    {LoadAll();}

  function LoadAll(){
    document.getElementById("demo").innerHTML = "Success!";
    document.getElementById("imgFirstAnswer").src = f(img_fa);
    document.getElementById("fa_txt").innerHTML = A_Decode("HNqatbp4wxqzfvfvwstbfvp4wwqztgtgp4wxfvtbqzrfgbp4ynazfvp4hnqafvtbtbp4wwtbwsfvrvp4tgwshnhntgtbp4fvtbechnqzujumtgrrp4hnqawsujumgb,,p4azsxsxazgbwshntbp4ynfvazyhp4hnqatbp4gbwsumuj..p4UMwsqqtbp4tbyhp4qzp4tgazazrf!!");
    document.getElementById("FirstAnswer").style.display = "block";

    document.getElementById("SecondAnswer").style.display = "block";
    document.getElementById("DecodedMessage").innerHTML = A_Decode("WS''qqtbp4ecazyhtbp4qzp4tgazujump4wwqzrrp4qzujrvp4qaqzqqtbp4yhqzujrrp4sxtgqzectbgbp4gbhnwstgtgp4hnazp4umaz");
  }

</script>
