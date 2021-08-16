---
title: Printing Triangle of Asterisks
---

## Purpose:

 <p>The purpose of this exercise is to rearrange code steps that prints triangle using asterisks. 
  This exercise will improve your understanding of how to write programs that involve nested loop.</p>


## Directions :

<div style="text-align: justify">
    <p>The following program prints triangle using asterisks. 
      However, the blocks have been mixed up and include one extra block that isn't needed in the solution. 
      Drag the blocks from the top and place them in the correct order on the bottom. 
      Click on Get Feedback to see if you are right.</p>

<div id="5-sortableTrash" class="sortable-code"></div> 
<div id="5-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="5-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="5-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "public class NextedTest{\n" +
    "    public static void main(String args[]){\n" +
    "        for(int x = 0; x &lt; 10; x++){\n" +
    "            for(int y = 0; y &lt; x +1; y++){\n" +
    "                System.out.println(&quot;*&quot;);\n" +
    "            }\n" +
    "            System.out.println();        \n" +
    "        }\n" +
    "    }\n" +
    "}\n" +
    "for (int y = 0; y &lt;= 5; y++){ #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "5-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "trashId": "5-sortableTrash"
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
