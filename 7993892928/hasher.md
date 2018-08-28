---
title: Hasher
---

<div style="text-align:center">
  <form id="HashCheck" onSubmit="hash(); return false;">
    <input type="text" id="answer" name="user_name" />
    <input type="button" value="Check" onclick="hash(); return false;" />
  </form>
</div>

<div id="result" style="text-align:center">
  Hash Result
</div> 

<hr>

<div style="text-align:center">
  <form id="Encode" onSubmit="A_Encode(); return false;">
    <input type="text" id="enc" />
    <input type="button" value="Encode" onclick="A_Encode(); return false;" />
  </form>
</div>

<div id="enc_result" style="text-align:center">
  Encode Result
</div> 

<script>
//BEING SNEAKY FOR NO REASON
function hash() {
    var InString = document.getElementById("HashCheck").elements[0].value
    var hash = 5381;
    for(var i = 0; i < InString.length; i++)
    {
       hash = hash*33 + InString.charCodeAt(i);
    }
    document.getElementById("result").innerHTML = hash;
    return hash;
}

var di = {};
di['a'] = "qz"; di['A'] = "QZ"; 
di['b'] = "wx"; di['B'] = "WX"; 
di['c'] = "ec"; di['C'] = "EC"; 
di['d'] = "rv"; di['D'] = "RV"; 
di['e'] = "tb"; di['E'] = "TB"; 
di['f'] = "yn"; di['F'] = "YN"; 
di['g'] = "um"; di['G'] = "UM"; 
di['h'] = "qa"; di['H'] = "QA"; 
di['i'] = "ws"; di['I'] = "WS"; 
di['j'] = "ed"; di['J'] = "ED"; 
di['k'] = "rf"; di['K'] = "RF"; 
di['l'] = "tg"; di['L'] = "TG"; 
di['m'] = "yh"; di['M'] = "YH"; 
di['n'] = "uj"; di['N'] = "UJ"; 
di['o'] = "az"; di['O'] = "AZ"; 
di['p'] = "sx"; di['P'] = "SX"; 
di['q'] = "dc"; di['Q'] = "DC"; 
di['r'] = "fv"; di['R'] = "FV"; 
di['s'] = "gb"; di['S'] = "GB"; 
di['t'] = "hn"; di['T'] = "HN"; 
di['u'] = "jm"; di['U'] = "JM"; 
di['v'] = "qq"; di['V'] = "QQ"; 
di['w'] = "ww"; di['W'] = "WW"; 
di['x'] = "ee"; di['X'] = "EE"; 
di['y'] = "rr"; di['Y'] = "RR"; 
di['z'] = "tt"; di['Z'] = "TT"; 

var rdi = {};
for (var prop in di) {
  if(di.hasOwnProperty(prop)) {
    rdi[di[prop]] = prop;
  }
}

function A_Encode()
{
  var StringToEncode = document.getElementById("Encode").elements[0].value
  var EncodedString = "";
  for (var i = 0; i < StringToEncode.length; i++) {
    var ThisChar = StringToEncode.charAt(i);
    if(di.hasOwnProperty(ThisChar)) 
    {
      EncodedString = EncodedString + di[ThisChar];
    } else {
      EncodedString = EncodedString + ThisChar + ThisChar;
    }
  }
  document.getElementById("enc_result").innerHTML = EncodedString;
  return EncodedString;
}


</script>
