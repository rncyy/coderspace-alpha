<!-- Data and Script -->
<script>
    import Navbar from "../../components/Navbar.svelte";
    import LessonTemplate from "../../components/LessonTemplate.svelte";
    import QuestionCard from "../../components/QuestionCard.svelte";
    import NavigationButton from "../../components/NavigationButton.svelte";
    let subtext = "Let's learn how the Do While: \"Do While\""
    let code = [
		"// DoWhileLoop.java\n" +
        "do {\n" +
		"\t // statements \n" +
        "} while (condition);",
		
		"// another example\n" +
        "int j = 7;\n" +
        "\tdo {\n" +
        "\tSystem.out.printn(“value: ” + j);\n" +
        "\tj++;\n" +
        "} while (x < 7);",
		
		"//DoWhile.java\n" +
        "public class Do While {\n" +
        "\tpublic static void main (String [] args) {\n" +
		"\t\tint q = 1;\n" +
		"\t\tdo {\n" +
		"\t\t\tSystem.out.println(q); \n" +
		"\t\t\tq++;\n" +
        "\t\t} while (q < 5);\n" +
		"\t}\n" +
        "}", // output: 1 2 3 4 5
    ];
    let question =
        "int w = 9;\n" +
        "do {\n" +
        "\tSystem.out.println(_____);\n" +
        "\tw--;\n" +
        "} while (w > 1);";

    let questionCardProps = {
        lessonTitle: "Do While Loop in Java",
        questionTitle: "Print out the value of the iterator variable",
        correctAnswer: "w",
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
<LessonTemplate lessonName="Do While Loop in Java" imageName="cmd" subtext={subtext}>
    <div class="content">
        <h2 class="questrial">What is Do While Loop</h2>
        <img src="https://static.javatpoint.com/images/java-loops.png" width="500" alt="java" class="mb-3 d-block mx-auto"/>
        <p class="work-sans light-text adjust-text">
            The do while loop is also similar in while loop, but it has a difference in the while loop. The Java do while loop is a control flow statement that runs a portion of a program at least once before continuing to run it based on a boolean condition.
        </p>
        <p class="work-sans light-text adjust-text">
            The part of the program will iterate several times with the use of do while loop, and if there is some number in your code that is not fixed and you need to execute your code at least once, you can use the do while loop.
        </p>
        <p class="work-sans light-text adjust-text">
            If the statement is true, it will back to the top to do statements execute again and will repeat until the statement become false. Let’s take a look in the syntax below:
        </p>
        <pre class=adjust-text>
            <code class="language-java">
                {code[0]}
            </code>
        </pre>
        <p class="work-sans light-text adjust-text">
           And now we see the syntax of the do while loop, let’s take a look this code that now have a condition and the statements.
        </p>
        <pre class=adjust-text>
            <code class="language-java">{code[1]}</code>
        </pre>
        <p class="work-sans light-text adjust-text">
            The body of the loop will be executed first the <code> while (x > 7) </code>. If the condition is true, the body of the loop inside the do statement will be executed again, the condition will be execute again and until this process will become false and the loop will stops.
        </p>
        <div class="alert alert-primary adjust-text d-flex align-items-center" role="alert">
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
            And this is how the do while loop works. 
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
                <a href="https://beginnersbook.com/2015/03/do-while-loop-in-java-with-example/">Beginners
                Book</a><br>
                <a href="https://www.programiz.com/java-programming/do-while-loop">Programmiz</a><br>
                <a href="https://www.javatpoint.com/java-do-while-loop">Java Point</a>
            </div>
        </div>
    </div>
    <div style="height: 3rem"></div>

    <!-- refer to the route list sent in GC -->
    <NavigationButton isFirstLesson={false} isLastLesson={false} prevLesson="iteration-structure-1" nextLesson="iteration-structure-3"/>
    <div style="height: 3rem"></div>
</LessonTemplate>


<!-- Scope Styles -->
<style>
    .adjust-text {
        margin-left: 20px;
    }
</style>