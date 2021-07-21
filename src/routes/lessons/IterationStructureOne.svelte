<!-- Data and Script -->
<script>
    import Navbar from "../../components/Navbar.svelte";
    import LessonTemplate from "../../components/LessonTemplate.svelte";
    import QuestionCard from "../../components/QuestionCard.svelte";
    import NavigationButton from "../../components/NavigationButton.svelte";
    let question =
        "int g = 3;\n" +
        "while (_____) {\n" +
        "\tSystem.out.println(g);\n" +
        "\tg++;\n" +
        "}"

    let subtext = "Let's learn how the While loop goes: \"While Loop\""
    let code = [
		"// WhileLoop.java\n" +
        "while (condition) {\n" +
		"\t // statements \n" +
        "}",
		
		"// another example\n" +
        "int s = 5;\n" +
        "\twhile (s > 1) {\n" +
        "\tSystem.out.println(s);\n" +
        "\ts++\n" +
        "}",
		
		"//While.java\n" +
        "public class While {\n" +
        "\tpublic static void main (String [] args) {\n" +
		"\tint k = 10;\n" +
		"\twhile (k > 1) {\n" +
		"\tSystem.out.println(k); \n" +
		"\tk++ \n" +
		"\t}\n" +
		"\t}\n" + 
        "}", //output: 1 2 3 4 5 6 7 8 9 
    ];
    let questionCardProps = {
        lessonTitle: "While Loop in Java",
        questionTitle: "Fill in the blanks what are going to print (Note: Remove whitespace between answer.)",
        correctAnswer: "g>3",
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
    <div class="alert alert-primary d-flex align-items-center" adjust-text role="alert">
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
<LessonTemplate lessonName="While Loop in Java" imageName="cmd" subtext={subtext}>
    <div class="content">
        <h2 class="questrial">What is While Loop</h2>
        <img src="https://static.javatpoint.com/images/java-loops.png" width="700" alt="java" class="mb-3 d-block mx-auto"/>
        <p class="work-sans light-text adjust-text">
            Loops are used to iterate or repeat the block of the code. If you want to code something, like want to show message 50 times you can use the loop and that is that is the purpose of it.
        </p>
        <p class="work-sans light-text adjust-text">
            So let's go learn the Iteration 1 and that is the While loop, the while loop is used to iterate or repeat the program again and again and used to run a code until it met the condition that you made.
        </p>
        <p class="work-sans light-text adjust-text">
            If the execution start and the condition returns true then the statement inside the while loop is well executed, and if the condition returns false then the statement inside the loop will stop. Let’s take a look in the syntax below: 
        </p>
        <pre class=adjust-text>
            <code class="language-java">
                {code[0]}
            </code>
        </pre>
        <p class="work-sans light-text adjust-text">
           And now we see the syntax of the while loop, let’s take a look this code that now have a condition and the statements.
        </p>
        <pre class=adjust-text>
            <code class="language-java">{code[1]}</code>
        </pre>
        <p class="work-sans light-text adjust-text">
            The condition inside the <code> while (s > 1)</code> will evaluates it, then if it’s true the code inside the loop will executed and then will continue again. Then when it became false the loop will stop. This is how the loop works, 1st iteration s = 1, condition = true, action 1 is printed and s will be increased to 2 and when it increased to 6 the loop will stop.
        </p>
        <div class="alert alert-primary d-flex align-items-center" role="alert">
            <svg class="bi flex-shrink-0 me-2" width="24" height="24" role="img" aria-label="Info:"><use xlink:href="#info-fill"/></svg>
            <div class="work-sans light-text">
                For the next example, you will see here the <code> public class..</code> and the <code> main class </code>. And you will see how the structures of the code.
            </div>
        </div>
        <pre class=adjust-text>
            <code class="language-java">
                {code[2]}
            </code>
        </pre>
        <p class="work-sans light-text adjust-text">
            This is how we use the while loop, and we can see it’s easy to use. 
        </p>
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
                <a href="https://beginnersbook.com/2015/03/while-loop-in-java-with-examples/">Beginners
                Book</a><br>
                <a href="https://https://www.programiz.com/java-programming/do-while-loop">Programmiz</a>
            </div>
        </div>
    </div>
    <div style="height: 3rem"></div>

    <!-- refer to the route list sent in GC -->
    <NavigationButton isFirstLesson={false} isLastLesson={false} prevLesson="decision-structure-2" nextLesson="iteration-structure-2"/>
    <div style="height: 3rem"></div>
</LessonTemplate>


<!-- Scope Styles -->
<style>
    .adjust-text {
        margin-left: 20px;
    }
</style>