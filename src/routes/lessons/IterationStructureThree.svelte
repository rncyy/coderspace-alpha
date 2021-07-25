<!-- Data and Script -->
<script>
    import Navbar from "../../components/Navbar.svelte";
    import LessonTemplate from "../../components/LessonTemplate.svelte";
    import QuestionCard from "../../components/QuestionCard.svelte";
    import NavigationButton from "../../components/NavigationButton.svelte";
    let subtext = "Let's learn how the For loop works: \"For Loop\"";
    let question =
        "for (int o = 1; o <= 5; o++) {\n" +
        "\tSystem.out.println(_____);\n" +
        "}";
    let code = [
		"// ForLoop.java\n" +
        "for (statement 1, statement 2, statement 3) {\n" +
		"\t// code \n" +
        "}",
		
		"// another example\n" +
        "int b = 7;\n" +
        "for(int b = 1; b <= 6 ;  b++){ \n" +
        "\tSystem.out.printn(b);\n" +
        "}",
		
		"//For.java\n" +
        "public class For {\n" +
        "\tpublic static void main (String [] args) {\n" +
		"\t\tint m = 3;\n" +
		"\t\tfor (int m = 1; m <= n; m++) {\n" +
		"\t\t\tSystem.out.println(\"I Love You\"); \n" +
		"\t\t}\n" +
		"\t}\n" +
        "}", // output: I Love You I Love You I love You
    ];
    let questionCardProps = {
        lessonTitle: "For Loop in Java",
        questionTitle: "Print the out the numbers: 1 - 5",
        correctAnswer: "o",
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
<LessonTemplate lessonName="For Loop in Java" imageName="cmd" subtext={subtext}>
    <div class="content">
        <h2 class="questrial">What is For Loop</h2>
        <img src="https://static.javatpoint.com/images/java-loops.png" width="500" alt="java" class="mb-3 d-block mx-auto"/>
        <p class="work-sans light-text adjust-text">
            The java for loop command is used to repeat a block of code a set number of times.
        </p>
        <p class="work-sans light-text adjust-text">
            And if the iteration of the loop is fixed then you are recommended to use the for loop.
        </p>
        <p class="work-sans light-text adjust-text">
            There are 3 types of for loops in java.
        </p>
        <ol class="adjust-text work-sans light-text">
            <li>Simple For Loop - the simple for loop is also the same in C/C++. We can set the variable’s value, check the condition, and increment or decrease the value. In simple loop it consists 4 parts:
                <ul class="adjust-text work-sans light-text">
                    <li>initialization = when the loop begins, it executes the starting condition only once. We can either initialize the variable or use one that has already been initialized. It is an optional condition.
                    <li>condition = it's the second condition that's run every time the loop's condition is tested. It keeps running until the condition is false. It must return either true or false as a boolean value. It is an optional condition.
                    <li>statement = the loop's statement is performed every time the second condition is false.
                    <li>increment/ decrement = 	It increases or decreases the value of the variable. It is a optional condition.
                </ul>
            <li>For Each or Enhanced For Loop - in Java, the for-each loop is used to iterate over an array or collection. Because we don't have to increment the value or use subscript notation, it's easier to use than a standard for loop. It operates on the basis of elements rather than indexes. It returns each element in the defined variable one by one.
            <li>Labeled For Loop - each Java for loop can be given a name. We do this by placing label before the for loop. If we have nested for loops, it is useful to be able to break/continue certain for loops. Typically, the break and continue keywords only break/continue the innermost loop.
        </ol>
		<p class="work-sans light-text adjust-text">
			Let’s see the syntax below:
		</p>
        <pre class=adjust-text>
            <code class="language-java">
                {code[0]}
            </code>
        </pre>
        <p class="work-sans light-text adjust-text">
           And now we see the syntax of the for loop, let’s take a look this code that now have a condition and the statements.
        </p>
        <pre class=adjust-text>
            <code class="language-java">{code[1]}</code>
        </pre>
        <p class="work-sans light-text adjust-text">
            The first statement will be executed once before the code block will be executed and it will initializes / declares the variables. The second statement specifies the condition under which the code block will be executed and the third statement will executed every time after the code block run. 
        </p>
        <div class="alert alert-primary d-flex align-items-center" role="alert">
            <svg class="bi flex-shrink-0 me-2" width="24" height="24" role="img" aria-label="Info:"><use xlink:href="#info-fill"/></svg>
            <div class="work-sans light-text">
                And for the next <code> code.. </code> we will see how the <code> for loop </code> works.
            </div>
        </div>
        <pre class=adjust-text>
            <code class="language-java">
                {code[2]}
            </code>
        </pre>
        <p class="work-sans light-text adjust-text">
            And this is how the for loop works. 
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
                <a href="https://www.w3schools.com/java/java_for_loop.asp">W3 Schools</a><br>
                <a href="https://www.programiz.com/java-programming/for-loop">Programmiz</a><br>
                <a href="https://www.javatpoint.com/java-for-">Java Point</a>
            </div>
        </div>
    </div>
    <div style="height: 3rem"></div>

    <!-- refer to the route list sent in GC -->
    <NavigationButton isFirstLesson={false} isLastLesson={false} prevLesson="iteration-structure-2" nextLesson="array-1"/>
    <div style="height: 3rem"></div>
</LessonTemplate>


<!-- Scope Styles -->
<style>
    .adjust-text {
        margin-left: 20px;
    }
</style>