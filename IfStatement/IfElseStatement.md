---
title: Printing Even or Odd Number
---

## Purpose:

 <p>The purpose of this exercise is to practice rearranging code steps to find the largest of two numbers. This exercise will help you master the sequence of statements execution involving conditional statements such as if--else .</p>

## Directions :

<div style="text-align: justify">
    <p>The following program declares variables, then create a Scanner object to prompt a user to enter two numbers, finds the greatest/largest between the two numbers, then display the result on the screen, but the code is mixed up. Drag the blocks from the top and place them in the correct order on the bottom. Click on Get Feedback to see if you are right.</p>
 
 <p>In this exercise, you will only fix PART of the program, that is, the lines marked "FIX THIS PART".</p>
    <hr/>   
    <pre>
import java.util.Scanner;
public class JavaProgram{
    public static void main(String[] args){
	//FIX THIS PART!!!
    }
}
</pre>
 
<div id="2-sortableTrash" class="sortable-code"></div> 
<div id="2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="2-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="2-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "int a, b;\n" +
    "Scanner scan = new Scanner(System.in);\n" +
    "System.out.println(&quot;Enter Two Number: &quot;);\n" +
    "a = scan.nextInt();\n" +
    "b = scan.nextInt();\n" +
    "if(a &gt; b)\n" +
    "    System.out.print(&quot;Largest of Two Number is a = &quot; + a);\n" +
    "else\n" +
    "    System.out.print(&quot;Largest of Two Number is b = &quot; + b);";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "2-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "2-sortableTrash"
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
