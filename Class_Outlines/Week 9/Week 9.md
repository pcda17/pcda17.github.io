## Week 9
<script  language="Javascript" type="text/javascript">
//cribbed from http://www.randomsnippets.com/2008/03/07/how-to-find-and-replace-text-dynamically-via-javascript/
var haystackText = "";
function findMyText(username) {
     var generic='/yourname/'
     username='/'+username+'/'
     if (haystackText.length == 0) {
          haystackText = document.getElementById("replace").innerHTML;
     }
     var match = new RegExp(generic, "ig");      
     var replaced = haystackText.replace(match, username);
     document.getElementById("replace").innerHTML = replaced;
}      

</script>
<p>Enter your username to customize code snippets below: &nbsp;<input id="username" name="username" type="text" size=14 onKeyUp="findMyText(document.getElementById('username').value);"></p>

<div id="replace">

#### Critical Text Analysis
Discuss readings for first 45 minutes.

#### Discussion
 Have students briefly present their work and discuss projects as a group.

#### Break

#### Exercise
Work on final project in class.