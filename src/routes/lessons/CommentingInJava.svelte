<!-- Data and Script -->
<script>
    import Navbar from "../../components/Navbar.svelte";
    import LessonTemplate from "../../components/LessonTemplate.svelte";
    import QuestionCard from "../../components/QuestionCard.svelte";
    import NavigationButton from "../../components/NavigationButton.svelte";
    let subtext = "Know the importance of describing and commenting on your code along with its practical implications and uses";
    let code = [
        "// put single line comment here",
		
        "// code for printing Hello World!\n" +
        "public class Main {\n" +
        "\tpublic static void main(String[] args) {\n" +
        "\t\tSystem.out.println(\"Hello World!\"); // prints Hello World!\n" +
        "\t}\n" +
        "}",
		
        "/* put\n" +
        "your\n" +
        "multi-line\n" +
		"comment\n" +
		"here */\n",
		
		"public class Main {\n" +
		"\t/*\n" +
        "\tmain() for printing Hello World!\n" +
        "\twelcome() for printing Welcome Java Programming!\n" +
		"\t*/\n" +
		"\tpublic static void main(String[] args) {\n" +
		"\t\tSystem.out.println(\"Hello World!\");\n" +
		"\t\twelcome();\n" +
		"\t}\n" +
		"\tpublic static void welcome(){\n" +
		"\t\tSystem.out.println(\"Welcome to Java Programming!\");\n" +
		"\t}\n" +
		"}",
		
		"/* put single line comment here */",
		
		"/**\n" +
        "*put\n" +
        "*your\n" +
		"*documentation\n" +
		"*comment\n" +
		"*here\n" +
		"*/",
		
		"public class FindSum {\n" +
		"\t/**\n" +
        "\t*welcome() used to find the sum of two integers\n" +
        "\t*@param num1 – first parameter to findSum\n" +
		"\t*@param num2 – second parameter to findSum/\n" +
		"\t*/\n" +
		"\tpublic int findSum(int num1, int num2) {\n" +
		"\t\treturn num1 + num2;" +
		"\t}\n" +
		"\tpublic static void main(String[] args) {\n" +
		"\t\tfindSum exmpl = new findSum();\n" +
		"\t\tint sum = exmpl.findSum(10,5);\n" +
		"\t\tSystem.out.println(“The Sum of 10 and 5 is: ” + sum);\n" +
		"\t}\n" +
		"}"
    ];
    let questionCardProps = {
    	lessonTitle: "Comments in Java",
        questionTitle: "Identify which type of comment is used in the code below. Use small caps only.",
        correctAnswer: "multi-line comment"
    }
</script>

<!-- HTML -->
<svg xmlns="http://www.w3.org/2000/svg" style="display: none;">
    <symbol id="check-circle-fill" fill="currentColor" viewBox="0 0 16 16">
        <path d="M16 8A8 8 0 1 1 0 8a8 8 0 0 1 16 0zm-3.97-3.03a.75.75 0 0 0-1.08.022L7.477 9.417 5.384 7.323a.75.75 0 0 0-1.06 1.06L6.97 11.03a.75.75 0 0 0 1.079-.02l3.992-4.99a.75.75 0 0 0-.01-1.05z"/>
    </symbol>
    <symbol id="info-fill" fill="currentColor" viewBox="0 0 16 16">
        <path d="M8 16A8 8 0 1 0 8 0a8 8 0 0 0 0 16zm.93-9.412-1 4.705c-.07.34.029.533.304.533.194 0 .487-.07.686-.246l-.088.416c-.287.346-.92.598-1.465.598-.703 0-1.002-.422-.808-1.319l.738-3.468c.064-.293.006-.399-.287-.47l-.451-.081.082-.381 2.29-.287zM8 5.5a1 1 0 1 1 0-2 1 1 0 0 1 0 2z"/>
    </symbol>
    <symbol id="exclamation-triangle-fill" fill="currentColor" viewBox="0 0 16 16">
        <path d="M8.982 1.566a1.13 1.13 0 0 0-1.96 0L.165 13.233c-.457.778.091 1.767.98 1.767h13.713c.889 0 1.438-.99.98-1.767L8.982 1.566zM8 5c.535 0 .954.462.9.995l-.35 3.507a.552.552 0 0 1-1.1 0L7.1 5.995A.905.905 0 0 1 8 5zm.002 6a1 1 0 1 1 0 2 1 1 0 0 1 0-2z"/>
    </symbol>
</svg>
<!-- TEMPLATES
Heading
    <h2 class="questrial">HEADING</h2>
Image
    <img src="source.jpg" width="400" alt="java" class="mb-3 d-block mx-auto"/>
Content Paragraph
    <p class="work-sans light-text adjust-text">
        Contents
    </p>
Code Block
    <pre class="adjust-text">
        <code class="language-java">
            code.block(here);
        </code>
    </pre>
Alerts
    <div class="alert alert-primary d-flex align-items-center" role="alert">
        <svg class="bi flex-shrink-0 me-2" width="24" height="24" role="img" aria-label="Info:"><use xlink:href="#info-fill"/></svg>
        <div class="work-sans light-text">
            Alert text
        </div>
    </div>
References
    <div class="references">
        <h2 class="questrial">References</h2>
        <a href="sources.html">Title</a>
    </div>
-->
<Navbar/>
<LessonTemplate lessonName="Commenting in Java" imageName="comment" subtext={subtext}>
    <div class="content">
		<img src="https://data-flair.training/blogs/wp-content/uploads/sites/2/2018/04/Types-of-comments-in-Java-1200x675.jpg" width="500" alt="java" class="mb-3 d-block mx-auto"/>
		<p class="work-sans light-text adjust-text">
            Any software would not be complete without comments. Comments in a program help to make it more human readable by putting the details of the code involved, and effective use of comments makes maintenance and bug discovery easier. 
        </p>
		<p class="work-sans light-text adjust-text">
            The Java comments are assertions that the compiler and interpreter do not execute. Comments can be used to provide more information or explanations about a variable, method, class, or statement. It can be used to conceal the program code as well.
        </p>
        <h2 class="questrial">Types of Comments</h2>
        <p class="work-sans light-text adjust-text">
            In Java, there are three types of comments:
        </p>
		<ol class="work-sans light-text adjust-text">
			<li>
				<h3 class="questrial">Single-line comments</h3>
				<p class="work-sans light-text adjust-text">
					It is used to comment on one line only. For illustrating the code functionality, a beginner level programmer generally employs single-line comments. It is one of the simplest comments to type.
				</p>
				<p class="work-sans light-text adjust-text">
					You can put your comment after ‘//’. See the syntax below.
				</p>
				<p class="work-sans light-text adjust-text">
					Syntax:
				</p>
				<pre class="adjust-text">
					<code class="language-java">
						{code[0]}
					</code>
				</pre>
				<p class="work-sans light-text adjust-text">
					Example:
				</p>
				<pre class="adjust-text">
					<code class="language-java">
						{code[1]}
					</code>
				</pre>
			</li>
			
			<li>
				<h3 class="questrial">Multi-line comments</h3>
				<p class="work-sans light-text adjust-text">
					Multiple lines of code can be commented with the multi-line comment. Because it is hassle to use ‘//’ at every line to describe a full method in a code or a complex snippet. To get around this, you can utilize multi-line comments.
				</p>
				<p class="work-sans light-text adjust-text">
					You can put your comment between ‘/*’ and ‘*/’. See the syntax below.
				</p>
				<p class="work-sans light-text adjust-text">
					Syntax:
				</p>
				<pre class="adjust-text">
					<code class="language-java">
						{code[2]}
					</code>
				</pre>
				<p class="work-sans light-text adjust-text">
					Example:
				</p>
				<pre class="adjust-text">
					<code class="language-java">
						{code[3]}
					</code>
				</pre>
				<p class="work-sans light-text adjust-text">
					We may also use the above syntax to make single-line comments, as demonstrated below:
				</p>
				<pre class="adjust-text">
					<code class="language-java">
						{code[4]}
					</code>
				</pre>
			</li>
			
			<li>
				<h3 class="questrial">Documentation comments</h3>
				<p class="work-sans light-text adjust-text">
					This type of comment is commonly used while writing code for a project/software package because it aids in the generation of a documentation page for reference, which can be used to learn about the methods available, their parameters, and so on.
				</p>
				<p class="work-sans light-text adjust-text">
					See the syntax below:
				</p>
				<p class="work-sans light-text adjust-text">
					Syntax:
				</p>
				<pre class="adjust-text">
					<code class="language-java">
						{code[5]}
					</code>
				</pre>
				<p class="work-sans light-text adjust-text">
					Example:
				</p>
				<pre class="adjust-text">
					<code class="language-java">
						{code[6]}
					</code>
				</pre>
			</li>
		</ol>
		
        <h2 class="questrial">Quick Test</h2>
        
        <!-- Question Card Content inside the pre tag-->
        <QuestionCard {...questionCardProps}>
            <pre class="question">
				/*
	This is the main method
	which makes use the
	findSum method
*/
            </pre>
        </QuestionCard>
        
        <div style="height: 10px;"></div>
        <div class="references">
            <h2 class="questrial">References</h2>
			<div class="questrial">
				<a href="https://www.javatpoint.com/java-comments">Java T Point</a><br>
				<a href="https://www.geeksforgeeks.org/comments-in-java/">GeeksForGeeks</a>
			</div>
        </div>
    </div>
    <div style="height: 3rem"></div>

    <!-- refer to the route list sent in GC -->
    <NavigationButton isFirstLesson={false} isLastLesson={false} prevLesson="variables-in-java" nextLesson="operations-1"/>
    <div style="height: 3rem"></div>
</LessonTemplate>


<!-- Scope Styles -->
<style>
    .adjust-text {
        margin-left: 20px;
    }
</style>