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
  Result
</div> 

<script>

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

</script>
