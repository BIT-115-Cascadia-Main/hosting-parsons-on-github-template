---
title: Printing Integer Values in Ascending Order
---

## Purpose:

 <p>The purpose of this exercise is to practice rearranging code steps that prints all values from 20 to 30. 
  This exercise will reinforce your understanding of how and when to use while loop to solve problems.</p>


## Directions :

<div style="text-align: justify">
    <p> The following program segment should print out all the values from 20 to 30 (20, 21, 22, … 30). 
      However, the blocks have been mixed up. Drag the blocks from the top and place them in the correct order on the bottom. 
      Click on Get Feedback to see if you are right.</p>
  
  <div id="4-sortableTrash" class="sortable-code"></div> 
<div id="4-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="4-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="4-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "int x = 20;\n" +
    "while(x&lt;=30){\n" +
    "	System.out.println(x);\n" +
    "	x++;\n" +
    "}";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "4-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "trashId": "4-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#4-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#4-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
