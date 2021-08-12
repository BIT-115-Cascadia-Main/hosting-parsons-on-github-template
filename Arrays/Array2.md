---
title: Prints an integer array that is right shifted by one
---

## Purpose:

 <p>The purpose of this exercise is to give you opportunity to practice more with arrays. The program prints an integer array that is right shifted by 1. 
  Arranging these code blocks correctly will improve your understanding on how arrays work and different operations that can be performed on them.</p>


## Directions :

<div style="text-align: justify">
    <p> The following program prints an integer array that is right shifted by one - so [7, 9, 4, 6] prints [6, 7, 9, 4]. However, the blocks have been mixed up and includes one extra block that isn't needed in the solution. 
      Drag the blocks from the top and place them in the correct order on the bottom. Click on Get Feedback to see if you are right.</p>
  
  <div id="9-sortableTrash" class="sortable-code"></div> 
<div id="9-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="9-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="9-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "import java.util.Arrays;\n" +
    "public class shiftRight{\n" +
    "	public static void main(String[] args){\n" +
    "		int[] arr = {7, 9, 4, 6};\n" +
    "		int[] result = new int[arr.length];\n" +
    "		result[0] = arr[arr.length-1];\n" +
    "		for (int i = 0; i &lt; arr.length-1; i++) result[i+1] = arr[i];\n" +
    "		System.out.println(Arrays.toString(result));\n" +
    "	}\n" +
    "}\n" +
    "for (int i = 0; i &lt; arr.length; i++) result[i+1] = arr[i]; #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "9-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "trashId": "9-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#9-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#9-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
