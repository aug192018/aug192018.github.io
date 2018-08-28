---
title: Happy Birthday!
CustomReturn: false
---

<style type="text/css">
 table.center {
    margin-left: auto;
    margin-right: auto;
}
</style>

<div style="text-align:center">
 <table class="center" id="Locations">
 <tr>
   <td>
     <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d4710.025622366988!2d-75.70739115844336!3d45.41744562661835!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zNDXCsDI1JzAzLjMiTiA3NcKwNDInMTQuMiJX!5e0!3m2!1sen!2sca!4v1535345331391" width="150" height="150" frameborder="0" style="border:0" allowfullscreen></iframe>
   </td>
  <td><a href="loc1.html">Heart of Centretown</a></td>
 </tr>
 <tr>
  <td colspan = "2" id="testrow">
    test
  </td>
 </tr>
 <tr>
   <td>
     <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2800.3766625182943!2d-75.69416968476577!3d45.42190797910049!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zNDXCsDI1JzE4LjkiTiA3NcKwNDEnMzEuMSJX!5e0!3m2!1sen!2sca!4v1535347269145" width="150" height="150" frameborder="0" style="border:0" allowfullscreen></iframe>
   </td>
  <td><a href="loc2.htm">Confederation Park</a></td>
 </tr>
 <tr>
   <td>
     <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2800.4191206256223!2d-75.71378168476576!3d45.42105197910048!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zNDXCsDI1JzE1LjgiTiA3NcKwNDInNDEuNyJX!5e0!3m2!1sen!2sca!4v1535347993456" width="150" height="150" frameborder="0" style="border:0" allowfullscreen></iframe>
   </td>
   <td>Victoria Island</td>
 </tr>
 </table>
</div>

<style>
.mycenter {
    text-align:center;
}
</style>

<script src = "/7571101397556063/htools.js"></script>
<script>
  alert(document.cookie)
 
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
  
  function lazyHash(InString) {
      var hash = 5381;
      for(var i = 0; i < InString.length; i++)
      {
         hash = hash*33 + InString.charCodeAt(i);
      }
      return hash;
  }
 
  var loc1_cookie = getCookie("loc1_SecondAnswerCookie");
  if (lazyHash(loc1_cookie)  == 7571710509952919)
  {
    document.getElementById("testrow").innerHTML = A_Decode("WSp4qzyhp4gbhnfvazujump4qzgbp4qatbtgtg..");
  }
</script>
