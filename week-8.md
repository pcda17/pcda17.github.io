## Week 8
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

Provide collection of several hundred texts grouped by genre:
- news articles
- blog posts
- literary prose
- poetry
- scientific articles
- spam emails

Have students choose two or three categories to work with.

Using scikit-learn rain ML model using small number of texts and measure classification accuracy for remaining set.

Train model using more texts and see if there’s any improvement.

Compare models.

Look at mis-classified texts and discuss what features make them outliers.



#### Break

Demonstrate cluster analysis.


Sentiment analysis: Evaluate/classify Twitter data.


