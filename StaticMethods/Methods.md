







<div id="6-sortableTrash" class="sortable-code"></div> 
<div id="6-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="6-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="6-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "public class ConvertBetweenMF {\n" +
    "    public static void main(String[] args) 	{\n" +
    "        System.out.println(&quot;Feet\tMeters\t|\tMeters\tFeet&quot;);\n" +
    "		for(int feet=1,meters=20;feet&lt;=10&amp;&amp;meters&lt;=65;feet++,meters+=5)\n" +
    "		{\n" +
    "		    getMeters(feet);\n" +
    "			getFeet(meters);\n" +
    "		}\n" +
    "	}\n" +
    "	\n" +
    "	// given a value in feet (an int), convert it to meters (a double)\n" +
    "	public static void getMeters(int feet)\n" +
    "	{\n" +
    "		System.out.printf(&quot;%d\t%5.3f\t|&quot;, feet , 0.305 * feet );\n" +
    "	}\n" +
    "	\n" +
    "	// given a value in meters (an int), convert it to feet (a double)\n" +
    "	public static void getFeet(int meters)\n" +
    "	{\n" +
    "		System.out.printf(&quot;\t%d\t%5.3f\t\n&quot;, meters, 3.279 * meters );\n" +
    "	}\n" +
    "}";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "6-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en"
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
