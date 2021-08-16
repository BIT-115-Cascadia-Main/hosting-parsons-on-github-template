---
title: Printing Integer Values in Descending Order
---

## Purpose:

 <p>The purpose of this exercise is to practice rearranging code steps that prints a countdown from 15 to 0. 
  This exercise will reinforce your understanding of how and when to use for loop to solve problems.</p>

## Directions :

<div style="text-align: justify">
    <p> The following program segment should print a countdown from 15 to 0 (15, 14, 13, … 0). 
      However, the blocks have been mixed up and include one extra block that is not needed in a correct solution. 
      Drag the blocks from the top and place them in the correct order on the bottom. Click on Get Feedback to see if you are right.</p>
  
  <div id="5-sortableTrash" class="sortable-code"></div> 
<div id="5-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="5-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="5-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "public class{\n" +
    "	public static void main (String[] args){\n" +
    "		for(int i =15; i&gt;=0; i--)\n" +
    "			System.out.println(i);\n" +
    "	}\n" +
    "}\n" +
    "for(int i=15; i&gt;0; i--) #distractor";
  function displayErrors(fb) {
      if(fb.errors.length > 0) {
          alert(fb.errors[0]);
      }
  }     
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "5-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "trashId": "5-sortableTrash",
    'feedback_cb' : displayErrors
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#5-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#5-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
