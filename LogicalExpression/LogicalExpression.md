---
title: Print Your Speeding Fines
---

## Purpose:

 <p>The purpose of this exercise is to practice rearranging code steps that prints your fine if you are speeding. With this exercise, you will improve your understanding of how logical expressions are used to formulate complex decisions.</p>

## Directions :

<div style="text-align: justify">
    <p> The following program should print your fine if you are speeding. If you are going over 65 but less than 75 the fine is 50. If you are going at least 75 and less than 85 the fine is 100. Over that the fine is 200. However, the blocks have been mixed up and includes two extra blocks that aren't needed in the solution. Drag the blocks from the top and place them in the correct order on the bottom. Click on Get Feedback to see if you are right.</p>
 
 <div id="3-sortableTrash" class="sortable-code"></div> 
<div id="3-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="3-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="3-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "public class SpeedLimits{\n" +
    "	public static void main(String args[]){\n" +
    "		int speed = 87;\n" +
    " 		if (speed &gt;  65 || speed &lt; 75)\n" +
    "			System.out.println(&quot;50&quot;);\n" +
    "		else if (speed &gt;= 75 &amp;&amp; speed &lt; 85)\n" +
    "			System.out.println(&quot;100&quot;);\n" +
    "		else\n" +
    "			System.out.println(&quot;200&quot;);\n" +
    "	}\n" +
    "}\n" +
    "else if ( speed &gt;= 75 || speed &lt; 85) #distractor\n" +
    "if (speed &gt; 65 &amp;&amp; speed &lt; 75) #distractor";
    function displayErrors(fb) {
      if(fb.errors.length > 0) {
          alert(fb.errors[0]);
      }
  }     
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "3-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "trashId": "3-sortableTrash",
    'feedback_cb' : displayErrors
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#3-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#3-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
