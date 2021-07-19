---
title: Printing Even or Odd Number
---

## Purpose:

 <p>The purpose of this exercise is to practice the program flow and the sequence of statement executions using the conditional statements.</p>


## Directions :

<div style="text-align: justify">
    <p>The following program should print out “x is even” if the remainder of x divided by 2 is 0 and “x is odd” otherwise, but the code is mixed up. Drag the blocks from the left and place them in the correct order on the right. Click on Get Feedback to see if you are right.</p>
 
<div id="2-sortableTrash" class="sortable-code"></div> 
<div id="2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="2-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="2-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "import java.util.Scanner;\n" +
    "public class JavaProgram\n" +
    "{\n" +
    "    public static void main(String args[])\n" +
    "    {\n" +
    "        int a, b, big;\n" +
    "        Scanner scan = new Scanner(System.in);\n" +
    "		\n" +
    "        System.out.print(&quot;Enter Two Number : &quot;);\n" +
    "        a = scan.nextInt();\n" +
    "        b = scan.nextInt();\n" +
    "		\n" +
    "        if(a&gt;b)\n" +
    "        {\n" +
    "            big = a;\n" +
    "        }\n" +
    "        else\n" +
    "        {\n" +
    "            big = b;\n" +
    "        }\n" +
    "		\n" +
    "        System.out.print(&quot;Largest of Two Number is &quot; +big);\n" +
    "    }\n" +
    "}";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "2-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#2-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
