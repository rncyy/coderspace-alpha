<!-- Data and Script -->
<!--suppress HtmlUnknownAnchorTarget -->
<script>
    import Navbar from "../../components/Navbar.svelte";
    import LessonTemplate from "../../components/LessonTemplate.svelte";
    import QuestionCard from "../../components/QuestionCard.svelte";
    import NavigationButton from "../../components/NavigationButton.svelte";

    let subtext = "Learn how Java stores data and the types of data it stores.";
    let code = [
        "[dataType] [variableName] = [initialValue];",

        "public static void main(String[] args) {\n" +
        "\tint num = 10;\n" +
        "\tString name = \"CoderSpace Alpha\";\n" +
        "\tboolean isAvailable;\n" +
        "\tdouble moneyDepositDollar = 50.90;\n" +
        "}\n",

        "int number = 15;\n" +
        "System.out.println(number);\n" +
        "/* prints out 15 */",

        "int number = 15;\n" +
        "System.out.println(number);\n" +
        "/* prints out 15 */\n" +
        "System.out.println(\"number\");\n" +
        "/* prints out the word number */",

        "int number = 90;\n" +
        "String websiteName = \"CoderSpace Alpha\";\n" +
        "boolean isUpdated = true;\n" +
        "double moneyLeft = 10.25;\n" +
        "System.out.println(_____);",

        "double grade = 92.23;\n" +
        "System.out.println(grade);\n// Outputs 92.23\n" +
        "grade = 95.58;\n" +
        "System.out.println(grade);\n// Outputs 95.58"
    ];
    let questionCardProps = {
        lessonTitle: "Variables in Java",
        questionTitle: "Print out the value of the variable with type of String",
        correctAnswer: "websiteName"
    };
    let correctFeedback = "Nice work! You are ready for the next lesson!";
    let incorrectFeedback = "Try again. Take note of the letter capitalization in your answer";
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

<Navbar/>
<LessonTemplate lessonName="Variables in Java" imageName="variable" subtext={subtext}>
    <div class="content">
        <h2 class="questrial">What are variables?</h2>
        <img src="https://i0.wp.com/techvidvan.com/tutorials/wp-content/uploads/sites/2/2020/02/types-of-variables-in-java.jpg?w=802&ssl=1" width="500" alt="java" class="mb-3 d-block mx-auto"/>
        <p class="work-sans light-text adjust-text">
            Variables are storage of data inside Java, and almost to all programming languages. Being able to store data to use in your program is important to ensure that the experience of the users are dependent on what they enter. Being able to store data is also useful for computations and methods that is used in your program.
        </p>
        <h3 class="questrial">Types of variables by data stored</h3>
        <p class="work-sans light-text adjust-text">
            There are different types of variables considering the type of the values stored inside that variable. These types are not all of the types available, but is the most used in programming with Java.
        </p>
        <h4 class="questrial">Primitive Types</h4>
        <ol class="work-sans light-text adjust-text">
            <li>Integers (<code>int</code>) - Stores whole numbers either positive or negative</li>
            <li>Characters (<code>char</code>) - Stores single characters enclosed in single quotation marks (<code>''</code>)</li>
            <li>Boolean (<code>boolean</code>) - Holds a <code>true</code> or <code>false</code> value</li>
            <li>Double (<code>double</code>) - Holds a number with decimal places. </li>
        </ol>
        <h4 class="questrial">Reference Types</h4>
        <ol class="work-sans light-text adjust-text">
            <li>String (<code>String</code>) - Stores a stream of characters called strings</li>
        </ol>
        <h3 class="questrial">Types of variables by scope</h3>
        <p class="work-sans light-text adjust-text">
            There are also different types of variables considering the scope of that variable. These types will not be discussed thoroughly in this chapter for it is a more advanced topic.
        </p>
        <ol class="work-sans light-text adjust-text">
            <li>
                Local
                <ul>
                    <li>Local variables are those declared inside a constructor, method, or block.</li>
                    <li>Local variables can only be used inside the constructor, method, or block they are declared in</li>
                </ul>
            </li>
            <li>
                Instance
                <ul>
                    <li>These are variables declared inside a class</li>
                    <li>They are, by default, accessible anywhere inside the classes they are declared</li>
                    <li>They can be accessed by the instance name of an object (more on this on a future course)</li>
                </ul>
            </li>
            <li>
                Static
                <ul>
                    <li>These are variables declared inside a class</li>
                    <li>They are, by default, accessible anywhere inside the classes they are declared</li>
                    <li>The main difference between a static and an instance variable is that static variables are accessed via the class name (more on this on a future course)</li>
                </ul>
            </li>
        </ol>
        <h3 class="questrial">Declaring Variables</h3>
        <p class="work-sans light-text adjust-text">
            There are different ways to declare a variable in Java depending on its visibility or scope
        </p>
        <h4 class="questrial">Declaring Local Variables</h4>
        <p class="work-sans light-text adjust-text">
            For local scope variables, we use the following syntax:
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[0]}
            </code>
        </pre>

        <p class="questrial light-text adjust-text">
            <br>
            <strong>Examples</strong>
        </p>
        <p class="work-sans light-text adjust-text">
            In these examples, we are going to declare multiple variables in the local scope inside the <code>main()</code> method.
        </p>
        <ol class="work-sans light-text adjust-text">
            <li>
                Store any number in an <code>int</code> variable with the name <code>num</code>
                <ul>
                    <li><code>int num = 10;</code></li>
                </ul>
            </li>
            <li>
                Store the string <code>"CoderSpace Alpha"</code> inside the variable named <code>name</code>
                <ul>
                    <li><code>String name = "CoderSpace Alpha";</code></li>
                </ul>
            </li>
            <li>
                Declare a variable with the name <code>isAvailable</code>
                <ul>
                    <li><code>boolean isAvailable;</code></li>
                    <li>This variable is a considered as a boolean type by the context of the variable name (either available/<code>True</code> or not available/<code>False</code></li>
                </ul>
            </li>
            <li>
                Store the money deposited ($50.90) by a user in the variable <code>moneyDepositDollar</code>
                <ul>
                    <li><code>double moneyDepositDollar = 50.90;</code></li>
                    <li>The variable is considered as a double because of the context of money</li>
                </ul>
            </li>
        </ol>
        <p class="work-sans light-text adjust-text">
            Below is a completed example on what the declared variables look like in a method.
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[1]}
            </code>
        </pre>
        <div class="alert alert-primary d-flex align-items-center adjust-text" role="alert">
            <svg class="bi flex-shrink-0 me-2" width="24" height="24" role="img" aria-label="Info:"><use xlink:href="#info-fill"/></svg>
            <div class="work-sans light-text">
                You can go to <a href="https://www.onlinegdb.com/online_java_compiler" target="_blank">OnlineGDB</a> to try and write you own programs to test your knowledge!
            </div>
        </div>
        <h3 class="questrial">Showing data stored in variables</h3>
        <p class="work-sans light-text adjust-text">
            As mentioned by our <a href="/#/lessons/hello-world">previous lesson</a>, we can use <code>System.out.println()</code> to print out data to our console. We can use the same method with our variables.
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[2]}
            </code>
        </pre>
        <p class="work-sans light-text adjust-text">
            With the program above, we have declared the variable <code>number</code> and set the initial value to <code>15</code>. Afterwards, we used the <code>System.out.println()</code> to print out the value of the variable.
        </p>
        <p class="work-sans light-text adjust-text">
            Take note that we have not used double quotes because the value we want is the one stored in the variable. Take a look at a simple example demonstrating the difference.
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[3]}
            </code>
        </pre>
        <h3 class="questrial">Changing the value of a variable</h3>
        <p class="work-sans light-text adjust-text">
            To change the value of a variable, simply refer to the variable name and assign the new value.
        </p>
        <p class="work-sans light-text adjust-text">
            Look at the example code below to further enhance your understanding:
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[5]}
            </code>
        </pre>
        <h2 class="questrial">Quick Test</h2>
        <!-- Question Card Content inside the pre tag-->
        <QuestionCard {...questionCardProps} correctFeedback={correctFeedback} incorrectFeedback={incorrectFeedback}>
            <pre class="question">
                {code[4]}
            </pre>
        </QuestionCard>

        <div style="height: 10px;"></div>
        <div class="references">
            <h2 class="questrial">References</h2>
            <div class="questrial">
                <a href="https://www.w3schools.com/java/java_variables.asp">W3Schools - Java Variables</a><br>
                <a href="https://www.javatpoint.com/java-variables">Javatpoint - Java Variables</a>
            </div>
        </div>
    </div>
    <div style="height: 3rem"></div>

    <!-- refer to the route list sent in GC -->
    <NavigationButton isFirstLesson={false} isLastLesson={false} prevLesson="hello-world" nextLesson="commenting-in-java"/>
    <div style="height: 3rem"></div>
</LessonTemplate>


<!-- Scope Styles -->
<style>
    .adjust-text {
        margin-left: 20px;
    }
</style>