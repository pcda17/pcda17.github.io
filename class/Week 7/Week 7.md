## Week 7
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

## Topics to Cover

- Descriptive statistics using numpy Python module
- Creating graphs in the matplotlib Python module

- Visualization
	- Tutorial source
		- http://www.labri.fr/perso/nrougier/teaching/matplotlib/


Tutorial source for statistical tests on literary works:
- http://digitalhumanities.org/companion/view?docId=blackwell/9781405103213/9781405103213.xml&doc.view=print&chunk.id=ss1-4-4&toc.depth=1&toc.id=0




