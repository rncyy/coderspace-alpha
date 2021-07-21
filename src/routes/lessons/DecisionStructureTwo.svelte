<!-- Data and Script -->
<script>
    import Navbar from "../../components/Navbar.svelte";
    import LessonTemplate from "../../components/LessonTemplate.svelte";
    import QuestionCard from "../../components/QuestionCard.svelte";
    import NavigationButton from "../../components/NavigationButton.svelte";
    
	let question =
        "int num = 1;\n" +
        "switch (num) {\n" +
        "\tcase 1:\n" +
        "\t\tSystem.out.println(\"one\");\n" +
        "\t\t_____;\n" +
        "\tdefault:\n" +
        "\t\tSystem.out.println(\"invalid number\");\n" +
        "}";
    let code = [
        "if (condition1) {\n" +
        "\t\t// code to be executed if condition1 is true\n" +
		"\tif (condition2) {\n" +
		"\t\t// code to be executed if condition2 is true\n" +
		"\t}\n" +
		"}",
		
        "public class Main {\n" +
        "\tpublic static void main(String[] args) {\n" +
		"\t\tint num = 50;\n" +
		"\t\tif (num == 50) {\n" +
		"\t\t\tSystem.out.println(\"num is equal to 50\");\n" +
		"\t\t\tif (num < 100) {\n" +
		"\t\t\t\tSystem.out.println(“ and num is less than to 100”);\n" +
		"\t\t\t}\n" +
		"\t\t}\n" +
		"\t}\n" +
		"}",
        
		"num is equal to 50 " +
		"and num is less than to 100",
		
		"if (condition1) {\n" +
		"\t// code to be executed if condition1 is true\n" +
		"} else if (condition2) {\n" +
		"\t// code to be executed if condition1 is false\n" +
		"} else if (condition3) {\n" +
		"\t// code to be executed if the condition1 and condition2 is false\n" +
		"}\n" +
		".\n" +
		".\n" +
		"else {\n" +
		"\t// code to be executed if none of the conditions are met\n" +
		"}",
		
		"public class Main {\n" +
        "\tpublic static void main(String[] args) {\n" +
		"\t\tint age = 18;\n" +
		"\t\tif (age == 0) {\n" +
        "\t\t\tSystem.out.println(\"Invalid age\");\n" +
        "\t\t} else if (age < 18 && age > 0) {\n" +
		"\t\t\tSystem.out.println(\"You cannot enter.\");\n" +
		"\t\t} else if (age >= 60) {\n" +
		"\t\t\tSystem.out.println(\"You're too old.\");\n" +
		"\t\t} else {\n" +
		"\t\t\tSystem.out.println(\"You can enter.\");\n" +
        "\t}" +
		"\t}" +
		"}",
		
		"You can enter.",
		
		"switch (expression) {\n" +
		"\tcase a:\n" +
		"\t\t// code to be executed\n" +
		"\tbreak;\n" +
		"\tcase b:\n" +
		"\t\t// code to be executed\n" +
		"\tbreak;\n" +
		".\n" +
		".\n" +
		"\tcase n:\n" +
		"\t\t// code to be executed\n" +
		"\tbreak;\n" +
		"\tdefault:\n" +
		"\t\t// code to be executed\n" +
		"}",
		
		"public class Main {\n" +
        "\tpublic static void main(String[] args) {\n" +
		"\t\tint day = 3;\n" +
		"\t\tswitch (day) {\n" +
        "\t\t\tcase 1:\n" +
		"\t\t\t\tSystem.out.println(\"Monday\");\n" +
		"\t\t\tbreak;\n" +
		"\t\t\tcase 2:\n" +
		"\t\t\t\tSystem.out.println(\"Tuesday\");\n" +
		"\t\t\tbreak;\n" +
		"\t\t\tcase 3:\n" +
		"\t\t\t\tSystem.out.println(\"Wednesday\");\n" +
		"\t\t\tbreak;\n" +
		"\t\t\tcase 4:\n" +
		"\t\t\t\tSystem.out.println(\"Thursday\");\n" +
		"\t\t\tbreak;\n" +
		"\t\t\tcase 5:\n" +
		"\t\t\t\tSystem.out.println(\"Frinday\");\n" +
		"\t\t\tbreak;\n" +
		"\t\t\tcase 6:\n" +
		"\t\t\t\tSystem.out.println(\"Saturday\");\n" +
		"\t\t\tbreak;\n" +
		"\t\t\tdefault:\n" +
		"\t\t\t\tSystem.out.println(\"Sunday\");\n" +
        "\t\t}\n" +
		"\t}\n" +
		"}",
		
		"Wednesday",
    ];
    let subtext = "Need more decision structures for your program? Try out using nested loops and the switch statement!"
    let questionCardProps = {
        lessonTitle: "Switch and nested loops",
        questionTitle: "Fill in the blanks to complete the code.",
        correctAnswer: "break"
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
<LessonTemplate lessonName="Decision Structure 2" imageName="decision" subtext={subtext}>
    <div class="content">
        <h2 class="questrial">Nested if and switch statement</h2>
        <img src="http://tech.queryhome.com/?qa=blob&qa_blobid=3523000838666960937" width="500" alt="java" class="mb-3 d-block mx-auto"/>
        <p class="work-sans light-text adjust-text">
            Decision making in programming is similar to decision making in real life. In programming also we face some situations where we want a certain block of code to be executed when some condition is fulfilled.
        </p>
        <p class="work-sans light-text adjust-text">
            In this tutorial, we will continue the last statements on the previous lesson. We will look on three more statements which is the:
        </p>
		<ul class="work-sans light-text adjust-text">
			<li>
				Nested if statement
			</li>
			<li>
				if else if statement
			</li>
			<li>
				switch statement
			</li>
		</ul>
		<h3 class="questrial">Nested if statement</h3>
        <p class="work-sans light-text adjust-text">
            The nested if statement is when an if statement is wrapped inside another if statement.
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
		<p class="work-sans light-text adjust-text">
            Output:
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[2]}
            </code>
        </pre>
        <p class="work-sans light-text adjust-text">
            As you can see in the above example, both statements are the output because the value of the variable num is true otherwise it will be ignored if it did not met the set condition.
        </p>
		<h3 class="questrial">if else if statement</h3>
		<p class="work-sans light-text adjust-text">
            When we need to check multiple conditions, we utilize the <strong>if-else-if statement</strong>. We only have one <code>if</code> and one <code>else</code> in this statement, but we can have several <code>else if</code>. <strong>if else if ladder</strong> is another name for it. See the syntax below:
        </p>
		<p class="work-sans light-text adjust-text">
            Syntax:
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[3]}
            </code>
        </pre>
		<div class="alert alert-primary d-flex align-items-center" role="alert">
			<svg class="bi flex-shrink-0 me-2" width="24" height="24" role="img" aria-label="Info:"><use xlink:href="#info-fill"/></svg>
			<div class="work-sans light-text">
				Note: The most important thing to remember is that in an <strong>if-else-if statement</strong>, the corresponding set of words is performed as soon as the condition is met, while the remainder is disregarded. If none of the conditions are met, the statements included in the “else” clause are executed.
			</div>
		</div>
		<p class="work-sans light-text adjust-text">
            Example:
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[4]}
            </code>
        </pre>
		<p class="work-sans light-text adjust-text">
            Output:
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[5]}
            </code>
        </pre>
		<h3 class="questrial">switch statement</h3>
        <p class="work-sans light-text adjust-text">
            A multiway branch statement is the switch statement. It makes it simple to route execution to different areas of code based on the expression's value.
        </p>
		<p class="work-sans light-text adjust-text">
            Syntax:
        </p>
        <pre class="adjust-text">
            <code class="language-java">
				{code[6]}
			</code>
        </pre>
        <p class="work-sans light-text adjust-text">
            Rules to apply in a switch statement:
        </p>
		<ul class="work-sans light-text adjust-text">
			<li>
				<p>The variable used in a switch statement can only be integers, convertable integers (byte, short, char), strings and enums.</p>
			</li>
			<li>
				<p>Only one time is the switch expression evaluated.</p>
			</li>
			<li>
				<p>The expression's value is compared against the values in each case.</p>
			</li>
			<li>
				<p>Case values that are duplicated are not permitted.</p>
			</li>
			<li>
				<p>A case's value must be of the same data type as the switch's variable and must be either a constant or a literal.</p>
			</li>
			<li>
				<p>The break statement is used to end a statement sequence inside the switch.</p>
			</li>
			<li>
				<p>It's not necessary to use the default and break statement.</p>
			</li>
			<li>
				<p>When none of the other situations are true, the default case can be utilized to complete a task. In the default instance, no break is required.</p>
			</li>
		</ul>
		<p class="work-sans light-text adjust-text">
            Example:
        </p>
		<pre class="adjust-text">
            <code class="language-java">
				{code[7]}
			</code>
        </pre>
		<p class="work-sans light-text adjust-text">
            Output:
        </p>
		<pre class="adjust-text">
            <code class="language-java">
				{code[8]}
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
                <a href="https://beginnersbook.com/2017/08/if-else-statement-in-java/">BeginnersBook</a><br>
                <a href="https://www.geeksforgeeks.org/decision-making-javaif-else-switch-break-continue-jump/">GeeksForGeeks</a><br>
                <a href="https://www.w3schools.com/java/java_switch.asp">W3Schools</a>
            </div>
        </div>
    </div>
    <div style="height: 3rem"></div>

    <!-- refer to the route list sent in GC -->
    <NavigationButton isFirstLesson={false} isLastLesson={false} prevLesson="decision-structure-1" nextLesson="iteration-structure-1"/>
    <div style="height: 3rem"></div>
</LessonTemplate>


<!-- Scope Styles -->
<style>
    .adjust-text {
        margin-left: 20px;
    }
</style>