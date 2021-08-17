---
title: Converts measurements from meters to feet
---

## Purpose:

 <p>The purpose of this exercise is to practice rearranging code steps involving a method with a return value. This method converts meters to feet. Arranging these code blocks correctly is important to your understanding of writing codes in Java using static methods that return values to the main method .</p>

## Directions :

<div style="text-align: justify">
    <p> The following code segments use a method to convert measurements from meters to feet and the method is invoked from the main() method. Given a value in meters (an int), the method converts it to feet (a double). However, the blocks have been mixed up and includes one extra block that isn't needed in the solution. Drag the blocks from the top and place them in the correct order on the bottom. Click on Get Feedback to see if you are right.</p>

<div id="8-sortableTrash" class="sortable-code"></div> 
<div id="8-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="8-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="8-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "public class ConvertToFeet {\n" +
    "	public static void main(String[] args){\n" +
    "		System.out.println(&quot;Meters\t\tFeet&quot;);\n" +
    "		for(int meters=20;meters&lt;=65;meters+=5) {\n" +
    "    		System.out.printf(&quot;%d\t\t%6.3f&quot;, meters, getFeet(meters));\n" +
    "		}\n" +
    "	}\n" +
    "	public static double getFeet(int meters){\n" +
    "		return 3.279 * meters;\n" +
    "	}\n" +
    "}\n" +
    "System.out.printf(&quot;%d\t\t%6.3f&quot;, feet, getMeters(feet)); #distractor";
      function displayErrors(fb) {
      if(fb.errors.length > 0) {
          alert(fb.errors[0]);
      }
  }     
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "8-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "trashId": "8-sortableTrash",
    'feedback_cb' : displayErrors
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#8-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#8-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
