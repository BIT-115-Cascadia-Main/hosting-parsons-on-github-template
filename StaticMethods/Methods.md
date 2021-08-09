---
title: Converts measurements from feet to meters
---

## Purpose:

 <p>The purpose of this exercise is to practice rearranging code steps involving a method. This method converts feet to meters. Arranging these code blocks correctly is important to your understanding of writing codes in Java using static methods.</p>


## Directions :

<div style="text-align: justify">
    <p> The following program uses a method to convert measurements from feet to meters. Given a value in feet (an int), it converts it to meters (a double). However, the blocks have been mixed up and includes one extra block that isn't needed in the solution. Drag the blocks from the top and place them in the correct order on the bottom. Click on Get Feedback to see if you are right.</p>

<div id="6-sortableTrash" class="sortable-code"></div> 
<div id="6-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="6-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="6-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "public class ConvertToMeters {\n" +
    "    public static void main(String[] args) 	{\n" +
    "        System.out.println(&quot;Feet\tMeters&quot;);\n" +
    "        for(int feet=20;feet&lt;=65;feet+=5) getMeters(feet);\n" +
    "    }\n" +
    "    public static void getMeters(int feet) {\n" +
    "        System.out.printf(&quot;%d\t%5.3f\n&quot;, feet , 0.305 * feet );\n" +
    "    }\n" +
    "    \n" +
    "}\n" +
    "getFeet(meters) #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "6-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "trashId": "6-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#6-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#6-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
