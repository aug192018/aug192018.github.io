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

<!--//////////////////////-->

<hr>

<div style="text-align:center">
  <form id="Encode" onSubmit="T_Encode(); return false;">
    <input type="text" id="enc" />
    <input type="button" value="Encode" onclick="T_Encode(); return false;" />
  </form>
</div>

<div id="enc_result" style="text-align:center">
  Encode Result
</div> 

<!--//////////////////////-->

<hr>

<div style="text-align:center">
  <form id="Decode" onSubmit="T_Decode(); return false;">
    <input type="text" id="enc" />
    <input type="button" value="Decode" onclick="T_Decode(); return false;" />
  </form>
</div>

<div id="dec_result" style="text-align:center">
  Decode Result
</div> 

<!--//////////////////////-->
<!--//////////////////////-->
<!--//////////////////////-->
<!--//////////////////////-->

<script src="./7571101397556063/htools.js"></script>
