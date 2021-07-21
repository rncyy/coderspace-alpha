<!-- Data and Script -->
<script>
    import Navbar from "../../components/Navbar.svelte";
    import LessonTemplate from "../../components/LessonTemplate.svelte";
    import QuestionCard from "../../components/QuestionCard.svelte";
    import NavigationButton from "../../components/NavigationButton.svelte";
    let subtext = "Learn how the different assignment and logical operators work"
    let code = [
		"// Assignment.java\n" +
        "int y = 10;\n" +
		"int y += 10;\n" +
		"int y -= 10;\n" +
		"int y *= 10;\n" +
		"int y %= 10;\n" +
		"// Logical.java \n" +
        "// AND Operator\n" +
		"System.out.println((1 > 3) && (3 > 8)); \n" + // true
		"System.out.println((1 < 3) && (3 < 8)); \n" + // false
		"// OR Operator\n" +
		"System.out.println((1 < 3) || (3 > 8)); \n" + // true
		"System.out.println((8 < 3) && (3 < 10)); \n" + // false
		"// NOT Operator\n" +
		"System.out.println(!(5 > 9)); \n" + // true
		"System.out.println(!(8 < 10));", // false
		
		
		"// another example\n" +
		"// Asignment Operator\n" +
        "int j1 = 5;\nint j2 = 10;\n" +
        "System.out.println(“j1 = ” + j1);\n" +
        "System.out.println(“j2 = ” + j2);\n" +
		"j1 += j2;\n" +
		"System.out.println(“j1 = ” + j1);\n" +
        "//Logical Operator\n" + 
		"int a = 5;\nint b = 8;\nint c = 9;\n" +
		"if((a > b) && (b < c)) {\n" +
		"\tSystem.out.println(“Chan”);\n" +
		"} else {\n" +
		"\tSystem.out.println(“Sunwoo”);\n" +
		"}",
		
		
		"//Assign.java\n" +
        "public class Assign {\n" +
        "\tpublic static void main (String [] args) {\n" +
		"\t\tint k = 5;\n" +
		"\t\tint s  = 10;\n" +
		"\t\tk += s;\n" +
		"\t\tSystem.out.println(“k += ” + k); \n" +
		"\t\ts *= k; \n" +
		"\t\tSystem.out.println(“s *= ” + s); \n" +
		"\t}\n" +
        "}\n", // output: k = 15 s = 50

		"//Logic.java\n" +
		"public class Logic {\n" +
		"\tpublic static void main (String [] args) {\n" +
		"\tint k = 100, b = 40, c = 7;\n" +
		"\tif ((k < c ) || (b > k)) { \n" +
		"\tSystem.out.println(“true”); \n" +
		"\t}else { \n" +
		"\System.out.println(“false”); \n" +
		"\t}\n" +	
		"\t}\n" +
		"}",
		
    ];
    let questionCardProps = {
        lessonTitle: "Assignment Operator and Logical Operator",
        questionTitle: "Assign the difference between num1 and num2 to num3 using an assignment operator",
        correctAnswer: "-=",
		
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
<LessonTemplate lessonName="Operators 2" imageName="equals" subtext={subtext}>
    <div class="content">
        <h2 class="questrial">Asignment and Logical Operators</h2>
        <img src="https://python-tricks.com/wp-content/uploads/2020/08/operators-in-java.png" width="700" alt="java" class="mb-3 d-block mx-auto"/>
        <p class="work-sans light-text adjust-text">
            The symbols that execute operations on the variables and values are known as operators.
        </p>
        <p class="work-sans light-text adjust-text">
            So let’s about the assignment operators, it is used to assign values to variables. The assignment operator's left side assign the variable, 
			while the assignment operator's right side assign the value. Here is the <code>(=)</code> assignment operator. The logical operators are the
			one that tells whether an expression is true or false. Logical operators are being used in <code> Decision Making</code>. 
			Here’s the other assignment and logical operators:
        </p>
		<h3 class="questrial">
			Assignment Operators
		</h3>
        <table class="table work-sans light-text adjust-text">
			<thead>
				<tr>
					<th scope="col">Operator</th>
					<th scope="col">Example</th>
					<th scope="col">Equivalent to</th>
				</tr>
			</thead>
			<tbody>
				<tr>
					<td>=</td>
					<td>+=</td>
					<td>-=</td>
					<td>*=</td>
					<td>/=</td>
					<td>%=</td>
				</tr>
				<tr>
					<td>a = b;</td>
					<td>a += b;<td>
					<td>a -= b;</td>
					<td>a *= b;</td>
					<td>a /= b;</td>
					<td>a %= b;</td>
				</tr>
				<tr>
					<td>a = b;</td>
					<td>a = a + b;</td>
					<td>a = a - b;</td>
					<td>a = a * b;</td>
					<td>a = a / b;</td>
					<td>a = a % b;</td>
				</tr>
			</tbody>
		</table>
		<h3 class="questrial">
			Logical Operators
		</h3>
        <table class="table work-sans light-text adjust-text">
			<thead>
				<tr>
					<th scope="col">Operator</th>
					<th scope="col">Example</th>
					<th scope="col">Meaning</th>
				</tr>
			</thead>
			<tbody>
				<tr>
					<td>&& (Logical AND)</td>
					<td>|| (Logical OR)</td>
					<td>! (Logical NOT)</td>
				</tr>
				<tr>
					<td>expression1 && expression2</td>
					<td>expression1 || expression2</td>
					<td>!expression</td>
				</tr>
				<tr>
					<td>true only if both expression1 and expression2 are true</td>
					<td>true if either expression1 or expression2 is true</td>
					<td>true if expression is false and vice versa</td>
				</tr>
			</tbody>
		</table>
		<p class="work-sans light-text adjust-text">
			Let’s see the syntax below:
		</p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[0]}
            </code>
        </pre>
        <p class="work-sans light-text adjust-text">
           This is how it looks when you are using the assignment operators and logical operators. Let’s take a look this code:
        </p>
        <pre class="adjust-text">
            <code class="language-java">{code[1]}</code>
        </pre>
        <p class="work-sans light-text adjust-text">
            We use the assignment operator to display the 2 value the j1 and the j2 and the next thing 
			that we do is we add them both and display the assigned value. This is how we code the logical operator, using the and, 
			or and not operator. AND if the both expression is true, OR if one of the expression is true and NOT true if the expression 
			is fall and vice versa.
        </p>
        <div class="alert alert-primary d-flex align-items-center adjust-text" role="alert">
            <svg class="bi flex-shrink-0 me-2" width="24" height="24" role="img" aria-label="Info:"><use xlink:href="#info-fill"/></svg>
            <div class="work-sans light-text">
                And the next example is we will see how the <code> assignment operator </code> and <code> logical operators </code> work 
				and the result of it. In logical operator we use the if else statement because it checks the boolean condition if it’s true or false.
            </div>
        </div>
        <pre class="adjust-text">
            <code class="language-java">
                {code[2]}
            </code>
        </pre>
        <p class="work-sans light-text adjust-text">
            So here’s how the assignment operators code looks like. We can easily add, minus, multiply etc when applying the assignment operator. And in the logical operator 
			we use the boolean algebra to know the if its true or false.
        </p>
        <h2 class="questrial">Quick Test</h2>
        
        <!-- Question Card Content inside the pre tag-->
        <QuestionCard {...questionCardProps}>
            <pre class="question">
int num1 = 30;
int num2 = 40;
int num3 = 0;
num3 = num1 _____ num2;
            </pre>
        </QuestionCard>
        
        <div style="height: 10px;"></div>
        <div class="references">
            <h2 class="questrial">References</h2>
			<div class="questrial">
				<a href="https://www.programiz.com/java-programming/operators">Programmiz</a><br>
				<a href="https://www.geeksforgeeks.org/java-assignment-operator-with-examples/">Geeks for Geeks</a><br>
				<a href="https://www.tutorialspoint.com/java/java_assignment_operators_examples.htm">Tutorial
					Point</a><br>
				<a href="https://www.scientecheasy.com/2020/05/logical-operators-in-java.html/">Scientecheasy</a>
			</div>
        </div>
    </div>
    <div style="height: 3rem"></div>

    <!-- refer to the route list sent in GC -->
    <NavigationButton isFirstLesson={false} isLastLesson={false} prevLesson="operations-1" nextLesson="decision-structure-1"/>
    <div style="height: 3rem"></div>
</LessonTemplate>


<!-- Scope Styles -->
<style>
    .adjust-text {
        margin-left: 20px;
    }
</style>