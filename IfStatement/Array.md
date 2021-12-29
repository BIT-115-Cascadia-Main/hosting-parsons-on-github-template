---
title: Prints even elements of an array
---

## Purpose:

 <p>The purpose of this exercise is to practice rearranging code steps involving an array. The program segment prints each even element of the array. 
  Arranging these code blocks correctly is important to your understanding of how to create, initialize, access, and display elements of an array.</p>

## Directions :

<div style="text-align: justify">
    <p> The following program segment prints each element in the array that is even. However, the blocks have been mixed up and includes one extra block that isn't needed in the solution. 
      Drag the blocks from the top and place them in the correct order on the bottom. Click on Get Feedback to see if you are right.</p>
  
  <div id="8-sortableTrash" class="sortable-code"></div> 
<div id="8-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="8-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="8-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "import java.util.Scanner;\n" +
    "public class JavaProgram {\n" +
    "    public static void main(String args[]) {\n" +
    "        int a, b, big;\n" +
    "        Scanner scan = new Scanner(System.in);\n" +
    "        System.out.print(&quot;Enter Two Number : &quot;);\n" +
    "        a = scan.nextInt();\n" +
    "        b = scan.nextInt();\n" +
    "        if(a&gt;b)\n" +
    "        {\n" +
    "            big = a;\n" +
    "        }\n" +
    "        else\n" +
    "        {\n" +
    "            big = b;\n" +
    "        }\n" +
    "        System.out.print(&quot;Largest of Two Number is &quot; +big);\n" +
    "    }\n" +
    "}";
  function displayErrors(fb) {
      if(fb.errors.length > 0) {
          alert("• " + fb.errors.join("\n\n• "));
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
