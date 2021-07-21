<!-- Data and Script -->
<script>
    import Navbar from "../../components/Navbar.svelte";
    import LessonTemplate from "../../components/LessonTemplate.svelte";
    import QuestionCard from "../../components/QuestionCard.svelte";
    import NavigationButton from "../../components/NavigationButton.svelte";
    
	let subtext = "Let your program make its own decisions through the decision structures in Java!"
    let code = [
        "if (condition) {\n" +
        "\t// code to be executed if the condition is true\n" +
		"}",
		
        "public class Main {\n" +
        "\tpublic static void main(String[] args) {\n" +
		"\t\tint a = 11;\n" +
		"\t\tif (a > 10) {\n" +
        "\t\t\tSystem.out.println(\"value of a is greater than 10\")\n" +
        "\t\t}\n" +
        "\t}\n" +
		"}",
		
		"if (condition) {\n" +
        "\t// code to be executed if the condition is true\n" +
		"} else {\n" +
		"\t// code to be executed if the condition is false\n" +
		"}",
		
		"public class Main {\n" +
        "\tpublic static void main(String[] args) {\n" +
		"\t\tint a = 5;\n" +
		"\t\tif (a > 10) {\n" +
        "\t\t\tSystem.out.println(\"value of a is greater than 10\")\n" +
        "\t\t} else {\n" +
		"\t\t\tSystem.out.println(\"value of a is not greater than 10\")\n" +
        "\t}" +
		"}",
		
		"value of a is not greater than 10",
		
		"int a = (condition) ? expressionTrue : expressionFalse;"
    ];

	let question =
        "int age = 18;\n" +
        "if (age >= 18) {\n" +
        "\tSystem.out.println(\"Legal Age\");\n" +
        "} else {\n" +
        "\tSystem.out.println(\"Under Age\");\n" +
        "}";
    let questionCardProps = {
        lessonTitle: "Starting out with if and if...else",
        questionTitle: "Identify the output of the code below.",
        correctAnswer: "Legal Age"
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
    <pre>
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
<LessonTemplate lessonName="Decision Structure 1" imageName="decision" subtext={subtext}>
    <div class="content">
        <h2 class="questrial">if and if else statement in Java</h2>
        <img src="http://3.bp.blogspot.com/-fK4B2f5N3k8/T3VdIkIuAuI/AAAAAAAAAE4/2r7ouDq6pgU/s1600/if.jpg" width="700" alt="java" class="mb-3 d-block mx-auto"/>
        <p class="work-sans light-text adjust-text">
            Control flow statements are used when we need to execute a collection of statements based on a condition. For example, you want to know which number is greater than 1, if you entered the number 2 it will print “2 is greater than 1” while if you entered the number 0 it will print “0 is not greater than 1”.
        </p>
        <p class="work-sans light-text adjust-text">
            In this tutorial, we willl look at two different forms of control statements that you might use in Java programs depending on the situation. The following conditional statements will be covered in this tutorial:
        </p>
		<ul class="work-sans light-text adjust-text">
			<li>
				if statement
			</li>
			<li>
				if else statement
			</li>
		</ul>
		<h3 class="questrial">if statement</h3>
        <p class="work-sans light-text adjust-text">
            The if statement in Java is used to test the condition. If the condition is true, the if block is executed. If a condition is met, a statement or a collection of statements follows, as seen below:
        </p>
		<p class="work-sans light-text adjust-text">
            Syntax:
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[0]}
            </code>
        </pre>
		<div class="alert alert-primary d-flex align-items-center adjust-text" role="alert">
			<svg class="bi flex-shrink-0 me-2" width="24" height="24" role="img" aria-label="Info:"><use xlink:href="#info-fill"/></svg>
			<div class="work-sans light-text">
				Note: <code>if</code> is in lower case so when you write uppercase letters (If, IF), it will result to an error.
			</div>
		</div>
        <p class="work-sans light-text adjust-text">
            Example:
        </p>
		<pre class="adjust-text">
            <code class="language-java">
                {code[1]}
            </code>
        </pre>
		<p class="work-sans light-text adjust-text">
            In this example, the output will be <code>value of a is greater than 10</code> because the condition is true otherwise, the statement will be ignored. Only when the provided condition is true are the statements executed. The statements inside the if statement body are completely ignored if the condition is false.
        </p>
		<h3 class="questrial">if else statement</h3>
        <p class="work-sans light-text adjust-text">
            In if else statement, we can utilize an optional else block in this situation. If the test expression is false, the statements inside the body of the else block are performed. Below is how the if else statement looks like:
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
            Output:
        </p>
		<pre class="adjust-text">
            <code class="language-java">
				{code[4]}
			</code>
        </pre>
		<p class="work-sans light-text adjust-text">
            In the above example, we have a variable <code>a</code> that has a value of 5. In the if condition, it will test if the value of the variable a is greater than 10 or not. If the value is greater than 10, it will execute the statement inside the if otherwise, if the condition is false, the else statement is executed.
        </p>
		<p class="work-sans light-text adjust-text">
            We can also use the short hand if else which is known as the <strong>ternary operator</strong>. It consists of three operands. 
        </p>
		<p class="work-sans light-text adjust-text">
            Syntax:
        </p>
        <pre class="adjust-text">
            <code class="language-java">
				{code[5]}
			</code>
        </pre>
		
        <h2 class="questrial">Quick Test</h2>
        
        <!-- Question Card Content inside the pre tag-->
        <QuestionCard {...questionCardProps}>
            <pre class="question">
                {question}
            </pre>
        </QuestionCard>
        
        <div style="height: 10px;"></div>
        <div class="references">
            <h2 class="questrial">References</h2>
            <div class="questrial">
                <a href="https://www.w3schools.com/java/java_conditions.asp">W3Schools</a><br>
                <a href="https://www.programiz.com/java-programming/if-else-statement">Programiz</a>
            </div>
        </div>
    </div>
    <div style="height: 3rem"></div>

    <!-- refer to the route list sent in GC -->
    <NavigationButton isFirstLesson={false} isLastLesson={false} prevLesson="operations-2" nextLesson="decision-structure-2"/>
    <div style="height: 3rem"></div>
</LessonTemplate>


<!-- Scope Styles -->
<style>
    .adjust-text {
        margin-left: 20px;
    }
</style>