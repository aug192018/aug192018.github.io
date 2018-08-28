<div style="text-align:center">
  <form id="FirstQ" onSubmit="dogs(); return false;">
    <input type="text" id="answer" name="user_name" />
    <input type="button" value="Check" onclick="hash(); return false;" />
  </form>
</div>

<script>

function hash(InString) {
    var hash = 5381;
    for(var i = 0; i < InString.length; i++)
    {
       hash = hash*33 + InString.charCodeAt(i);
    }
    alert(hash)
    return hash;
}

</script>
