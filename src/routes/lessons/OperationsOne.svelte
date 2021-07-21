<!-- Data and Script -->
<script>
    import Navbar from "../../components/Navbar.svelte";
    import LessonTemplate from "../../components/LessonTemplate.svelte";
    import QuestionCard from "../../components/QuestionCard.svelte";
    import NavigationButton from "../../components/NavigationButton.svelte";
    let subtext = "Operate on different numbers and values with the several operators available in Java!"
    let code = [
        "public class Sum {\n" +
        "\tpublic static void main(String[] args) {\n" +
		"\t\tint sum1 = 25 + 10;\n" +
		"\t\tint sum2 = sum1 + 30;\n" +
		"\t\tint sum3 = sum2 + 5;\n" +
        "\t\tSystem.out.println(sum1);\n" +
        "\t\tSystem.out.println(sum2);\n" +
        "\t\tSystem.out.println(sum3);\n" +
        "\t}\n" +
        "}",
		
        "35\n" +
        "65\n" +
        "70",
        
        "public class Sum {\n" +
        "\tpublic static void main(String[] args) {\n" +
		"\t\tint sum1 = 1 + 2 + 3 + 4 + 5;\n" +
		"\t\tint sum2 = sum1 + 10 + 20;\n" +
        "\t\tSystem.out.println(sum1);\n" +
        "\t\tSystem.out.println(sum2);\n" +
        "\t}\n" +
        "}",
		
		"15\n" +
        "45",
		
		"public class Main {\n" +
        "\tpublic static void main(String[] args) {\n" +
		"\t\tint result = 50;\n" +
		"\t\tresult += 50;\n" +
        "\t\tSystem.out.println(result);\n" +
        "\t}\n" +
        "}",
		
		"100",
		
		"public class Diff {\n" +
        "\tpublic static void main(String[] args) {\n" +
		"\t\tint diff1 = 75 - 10;\n" +
		"\t\tint diff2 = diff1 - 21;\n" +
		"\t\tint diff3 = diff2 - 1;\n" +
        "\t\tSystem.out.println(diff1);\n" +
        "\t\tSystem.out.println(diff2);\n" +
        "\t\tSystem.out.println(diff3);\n" +
        "\t}\n" +
        "}",
		
		"65\n" +
        "44\n" +
        "43",
		
		"public class Diff {\n" +
        "\tpublic static void main(String[] args) {\n" +
		"\t\tint diff1 = 100 - 10 - 20 - 35;\n" +
		"\t\tint diff2 = diff1 - 20 - 20;\n" +
        "\t\tSystem.out.println(diff1);\n" +
        "\t\tSystem.out.println(diff2);\n" +
        "\t}\n" +
        "}",
		
		"35\n" +
        "-5",
		
		"public class Main {\n" +
        "\tpublic static void main(String[] args) {\n" +
		"\t\tint result = 50;\n" +
		"\t\tresult -= 50;\n" +
        "\t\tSystem.out.println(result);\n" +
        "\t}\n" +
        "}",
		
		"0",
		
		"public class Prod {\n" +
        "\tpublic static void main(String[] args) {\n" +
		"\t\tint prod1 = 5 * 10;\n" +
		"\t\tint prod2 = prod1 * 10;\n" +
		"\t\tint prod3 = prod2 * 2;\n" +
        "\t\tSystem.out.println(prod1);\n" +
        "\t\tSystem.out.println(prodf2);\n" +
        "\t\tSystem.out.println(prod3);\n" +
        "\t}\n" +
        "}",
		
		"50\n" +
        "500\n" +
        "1000",
		
		"public class Main {\n" +
        "\tpublic static void main(String[] args) {\n" +
		"\t\tint prod = 100 * 10 * 2 * 5;\n" +
        "\t\tSystem.out.println(prod);\n" +
        "\t}\n" +
        "}",
		
		"10000",
		
		"public class Main {\n" +
        "\tpublic static void main(String[] args) {\n" +
		"\t\tint result = 50;\n" +
		"\t\tresult *= 50;\n" +
        "\t\tSystem.out.println(result);\n" +
        "\t}\n" +
        "}",
		
		"2500",
		
		"public class Div {\n" +
        "\tpublic static void main(String[] args) {\n" +
		"\t\tint div1 = 100 / 5;\n" +
		"\t\tint div2 = div1 / 4;\n" +
		"\t\tint div3 = div2 / 5;\n" +
        "\t\tSystem.out.println(prod1);\n" +
        "\t\tSystem.out.println(prodf2);\n" +
        "\t\tSystem.out.println(prod3);\n" +
        "\t}\n" +
        "}",
		
		"20\n" +
        "5\n" +
        "1",
		
		"public class Main {\n" +
        "\tpublic static void main(String[] args) {\n" +
		"\t\tint div = 500 / 100 / 5;\n" +
        "\t\tSystem.out.println(div);\n" +
        "\t}\n" +
        "}",
		
		"1",
		
		"public class Main {\n" +
        "\tpublic static void main(String[] args) {\n" +
		"\t\tint result = 250;\n" +
		"\t\tresult /= 50;\n" +
        "\t\tSystem.out.println(result);\n" +
        "\t}\n" +
        "}",
		
		"5",
		
		"public class Mod {\n" +
        "\tpublic static void main(String[] args) {\n" +
		"\t\tint num = 15;\n" +
		"\t\tint mod = result % 7;\n" +
        "\t\tSystem.out.println(mod);\n" +
        "\t}\n" +
        "}",
		
		"1",
		
		"public class Mod {\n" +
        "\tpublic static void main(String[] args) {\n" +
		"\t\tint result = 11;\n" +
		"\t\tresult %= 4;\n" +
        "\t\tSystem.out.println(result);\n" +
        "\t}\n" +
        "}",
		
		"3",
		
		"public class PostInc {\n" +
        "\tpublic static void main(String[] args) {\n" +
		"\t\tint a = 10;\n" +
		"\t\tint b = a++;\n" +
        "\t\tSystem.out.println(b);\n" +
        "\t}\n" +
        "}",
		
		"11",
		
		"public class PreInc {\n" +
        "\tpublic static void main(String[] args) {\n" +
		"\t\tint a = 10;\n" +
		"\t\tint b = ++a;\n" +
        "\t\tSystem.out.println(b);\n" +
        "\t}\n" +
        "}",
		
		"11",
		
		"public class Main {\n" +
        "\tpublic static void main(String[] args) {\n" +
		"\t\tint a = 2;\n" +
		"\t\t// 2 will be printed then increment to 3\n" +
        "\t\tSystem.out.println(\"Post-increment: \" + a++);\n" +
		"\t\t// value of a is 3 then increment to 4\n" +
        "\t\tSystem.out.println(\"Pre-increment: \" + ++a);\n" +
        "\t}\n" +
        "}",
		
		"Post-increment: 2\n" +
		"Pre-increment: 4",
		
		"public class PostDec {\n" +
        "\tpublic static void main(String[] args) {\n" +
		"\t\tint a = 15;\n" +
		"\t\tint b = a--;\n" +
        "\t\tSystem.out.println(b);\n" +
        "\t}\n" +
        "}",
		
		"14",
		
		"public class PreDec {\n" +
        "\tpublic static void main(String[] args) {\n" +
		"\t\tint a = 15;\n" +
		"\t\tint b = --a;\n" +
        "\t\tSystem.out.println(b);\n" +
        "\t}\n" +
        "}",
		
		"14",
		
		"public class Main {\n" +
        "\tpublic static void main(String[] args) {\n" +
		"\t\tint a = 7;\n" +
		"\t\t// 7 will be printed then decrement to 6\n" +
        "\t\tSystem.out.println(\"Post-decrement: \" + a--);\n" +
		"\t\t// value of a is 6 then increment to 5\n" +
        "\t\tSystem.out.println(\"Pre-decrement: \" + --a);\n" +
        "\t}\n" +
        "}",
		
		"Post-increment: 7\n" +
		"Pre-increment: 5"
    ];
    let questionCardProps = {
    	lessonTitle: "Mathematical Operations in Java",
        questionTitle: "Identify the output of the code below.",
        correctAnswer: "9"
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
<LessonTemplate lessonName="Operations 1" imageName="plus" subtext={subtext}>
    <div class="content">
        <h2 class="questrial">Arithmetic and Comparison Operators</h2>
        <img src="https://python-tricks.com/wp-content/uploads/2020/08/operators-in-java.png" width="500" alt="java" class="mb-3 d-block mx-auto"/>
        <h3 class="questrial">Arithmetic Operators</h3>
		<p class="work-sans light-text adjust-text">
            Variables and values are operated on with the use of operators. These operators are <strong>mathematical operators</strong> that can be used to execute various simple and advanced arithmetic operations on the operands, which are <strong>primitive data types</strong>. These operators are made up of various unary and binary operators that can be used on one or two operands.
        </p>
        <p class="work-sans light-text adjust-text">
            Under the arithmetic operators, Java has a number of operators. See the table below:
        </p>
		
		<table class="table work-sans light-text adjust-text">
		  <thead class="thead-dark">
			<tr class="table-primary">
			  <th scope="col">Operator</th>
			  <th scope="col">Name</th>
			  <th scope="col">Description</th>
			  <th scope="col">Example</th>
			</tr>
		  </thead>
		  <tbody>
			<tr>
			  <th scope="row" class="table-primary">+</th>
			  <td>Addition</td>
			  <td>Adding two values</td>
			  <td>a + b</td>
			</tr>
			<tr>
			  <th scope="row" class="table-primary">-</th>
			  <td>Subtraction</td>
			  <td>Subtracting two values</td>
			  <td>a - b</td>
			</tr>
			<tr>
			  <th scope="row" class="table-primary">*</th>
			  <td>Multiplication</td>
			  <td>Multiplying two values</td>
			  <td>a * b</td>
			</tr>
			<tr>
			  <th scope="row" class="table-primary">/</th>
			  <td>Division</td>
			  <td>Dividing two values</td>
			  <td>a / b</td>
			</tr>
			<tr>
			  <th scope="row" class="table-primary">%</th>
			  <td>Modulo</td>
			  <td>Returns the division remainder</td>
			  <td>a % b</td>
			</tr>
			<tr>
			  <th scope="row" class="table-primary">++</th>
			  <td>Increment</td>
			  <td>Increases the value by 1</td>
			  <td>a++</td>
			</tr>
			<tr>
			  <th scope="row" class="table-primary">--</th>
			  <td>Decrement</td>
			  <td>Decreases the value by 1</td>
			  <td>a--</td>
			</tr>
		  </tbody>
		</table>
        <p class="work-sans light-text adjust-text">
            Now, let‘s take a look on each operator in Java:
        </p>
		<h3 class="questrial">Addition</h3>
		<p class="work-sans light-text adjust-text">
            Two values are added using the + operator. A combination of two constants, a constant and a variable, or a variable and a variable can be used.
        </p>
		<p class="work-sans light-text adjust-text">
            Example:
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[0]}
            </code>
        </pre>
		<p class="work-sans light-text adjust-text">
            Output:
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[1]}
            </code>
        </pre>
        <p class="work-sans light-text adjust-text">
            The value of 25 + 10 is stored or placed in the variable name <code>sum1</code>. Then in the next line, the value of <code>sum1</code> is added to 30 (a constant) which will result to the value of <code>sum2</code> and so on.
        </p>
        <p class="work-sans light-text adjust-text">
            Of course, you can make longer addition chains and hence add more than two values. Here's an example of combining three or more values.
        </p>
        <pre class="adjust-text">
            <code class="language-java">
				{code[2]}
			</code>
        </pre>
		<p class="work-sans light-text adjust-text">
            Output:
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[3]}
            </code>
        </pre>
        <p class="work-sans light-text adjust-text">
            Because adding a value to a variable is such a common action, Java has a built-in operator for it. It's the operator <code>+=</code>. Here's how to code using the <code>+=</code> operator:
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
		<p class="work-sans light-text adjust-text">
            The result variable is made equal to its own value (before being allocated the new value) + 50 in the second line of this example. This equals to 10 + 20.
        </p>
		<p class="work-sans light-text adjust-text">
            In this example, in the second line, the variable result adds 50. This also equivalent to the syntax, <code>result = result + 50;</code>
        </p>
		<h3 class="questrial">Subtraction</h3>
		<p class="work-sans light-text adjust-text">
            Subtracting one value from another is done with the - operator. This can be done by subtracting a constant from another constant, a constant from a variable, or a variable from another variable.
        </p>
		<p class="work-sans light-text adjust-text">
            Example:
        </p>
		<pre class="adjust-text">
            <code class="language-java">
                {code[6]}
            </code>
        </pre>
		<p class="work-sans light-text adjust-text">
            Output:
        </p>
		<pre class="adjust-text">
            <code class="language-java">
                {code[7]}
            </code>
        </pre>
		<p class="work-sans light-text adjust-text">
            The <code>-</code> operator will get the difference between the two values just like with the <code>+</code> operator at runtime.
        </p>
		<p class="work-sans light-text adjust-text">
            Of course, you can also make longer subtraction chains and hence subtract more than two values. Here's an example of combining three or more values.
        </p>
		<pre class="adjust-text">
            <code class="language-java">
                {code[8]}
            </code>
        </pre>
		<p class="work-sans light-text adjust-text">
            Output:
        </p>
		<pre class="adjust-text">
            <code class="language-java">
                {code[9]}
            </code>
        </pre>
		<p class="work-sans light-text adjust-text">
            Java has an operator for removing a value from a variable and assigning the result to the variable, just like it does for addition. Let’s take a look on the example using the <code>-=</code> operator:
        </p>
		<pre class="adjust-text">
            <code class="language-java">
                {code[10]}
            </code>
        </pre>
		<p class="work-sans light-text adjust-text">
            Output:
        </p>
		<pre class="adjust-text">
            <code class="language-java">
                {code[11]}
            </code>
        </pre>
		<h3 class="questrial">Multiplication</h3>
		<p class="work-sans light-text adjust-text">
            Multiplying one value from another is done with the * operator. This can be done by multiplying a constant from another constant, a constant from a variable, or a variable from another variable.
        </p>
		<p class="work-sans light-text adjust-text">
            Example:
        </p>
		<pre class="adjust-text">
            <code class="language-java">
                {code[12]}
            </code>
        </pre>
		<p class="work-sans light-text adjust-text">
            Output:
        </p>
		<pre class="adjust-text">
            <code class="language-java">
                {code[13]}
            </code>
        </pre>
		<p class="work-sans light-text adjust-text">
            The <code>*</code> operator will get the product between the two values just like with the other operators at runtime.
        </p>
		<p class="work-sans light-text adjust-text">
            Of course, you can also make longer multiplication chains and hence multiply more than two values. Here's an example of combining three or more values.
        </p>
		<pre class="adjust-text">
            <code class="language-java">
                {code[14]}
            </code>
        </pre>
		<p class="work-sans light-text adjust-text">
            Output:
        </p>
		<pre class="adjust-text">
            <code class="language-java">
                {code[15]}
            </code>
        </pre>
		<p class="work-sans light-text adjust-text">
            In Java applications, multiplying a variable with a value and then assigning the value back to the variable is a typical math operation. As a result, Java has an explicit operator for this task. The <code>*=</code> operator.
        </p>
		<pre class="adjust-text">
            <code class="language-java">
                {code[16]}
            </code>
        </pre>
		<p class="work-sans light-text adjust-text">
            Output:
        </p>
		<pre class="adjust-text">
            <code class="language-java">
                {code[17]}
            </code>
        </pre>
		<h3 class="questrial">Division</h3>
		<p class="work-sans light-text adjust-text">
            Dividing one value from another is done with the <code>/</code> operator. This can be done by dividing a constant from another constant, a constant from a variable, or a variable from another variable.
        </p>
		<p class="work-sans light-text adjust-text">
            Example:
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[18]}
            </code>
        </pre>
		<p class="work-sans light-text adjust-text">
            Output:
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[19]}
            </code>
        </pre>
		<p class="work-sans light-text adjust-text">
            The <code>/</code> operator will get the difference between the two values just like with the other operators at runtime.
        </p>
		<p class="work-sans light-text adjust-text">
            Of course, you can also make longer division chains and hence divide more than two values. Here's an example of combining three or more values.
        </p>
		<pre class="adjust-text">
            <code class="language-java">
                {code[20]}
            </code>
        </pre>
		<p class="work-sans light-text adjust-text">
            Output:
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[21]}
            </code>
        </pre>
		<p class="work-sans light-text adjust-text">
            In Java applications, dividing a variable with a value and then assigning the value back to the variable is a typical math operation. As a result, Java has an explicit operator for this task. The <code>/=</code> operator.
        </p>
		<pre class="adjust-text">
            <code class="language-java">
                {code[22]}
            </code>
        </pre>
		<p class="work-sans light-text adjust-text">
            Output:
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[23]}
            </code>
        </pre>
		<h3 class="questrial">Modulo</h3>
		<p class="work-sans light-text adjust-text">
            The remainder math operation divides one value by another in integer and returns the remainder of the division. The modulo operation is another name for the remainder operation. The % (percentage) character is the operator for the remainder/modulo operation.
        </p>
		<p class="work-sans light-text adjust-text">
            Example:
        </p>
		<pre class="adjust-text">
            <code class="language-java">
                {code[24]}
            </code>
        </pre>
		<p class="work-sans light-text adjust-text">
            Output:
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[25]}
            </code>
        </pre>
		<p class="work-sans light-text adjust-text">
            15 divided by 7 is 2 with a remainder of 1 (7 times 2 is 14). Thus, the remainder variable is assigned the value 1.
        </p>
		<p class="work-sans light-text adjust-text">
            A shortcut operator for dividing a variable by another value and allocating the remainder of that division to the variable is also available in Java. The <code>%=</code> operator. See the example below:
        </p>
		<pre class="adjust-text">
            <code class="language-java">
                {code[26]}
            </code>
        </pre>
		<p class="work-sans light-text adjust-text">
            Output:
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[27]}
            </code>
        </pre>
		<h3 class="questrial">Increment</h3>
		<p class="work-sans light-text adjust-text">
            Unlike the other operations, this is a unary operator that only works on one operand. It's a function that <strong>increases</strong> the value of an integer. It has two applications:
        </p>
		<ol class="work-sans light-text adjust-text">
			<li>
				<h4 class="questrial">Post-increment</h4>
				<p class="work-sans light-text adjust-text">
					The value of the operand is incremented when it is inserted after the variable name, but the previous value is preserved until the execution of this statement, and it is updated before the execution of the next statement. Adding of <code>++ after</code> the variable.
				</p>
				<p class="work-sans light-text adjust-text">
					Example:
				</p>
				<pre class="adjust-text">
					<code class="language-java">
						{code[28]}
					</code>
				</pre>
				<p class="work-sans light-text adjust-text">
					Output:
				</p>
				<pre class="adjust-text">
					<code class="language-java">
						{code[29]}
					</code>
				</pre>
			</li>
			<li>
				<h4>Pre-increment</h4>
				<p class="work-sans light-text adjust-text">
					The operand's value is instantly incremented when it is inserted before the variable name. Adding of <code>++ before</code> the variable.
				</p>
				<p class="work-sans light-text adjust-text">
					Example:
				</p>
				<pre class="adjust-text">
					<code class="language-java">
						{code[30]}
					</code>
				</pre>
				<p class="work-sans light-text adjust-text">
					Output:
				</p>
				<pre class="adjust-text">
					<code class="language-java">
						{code[31]}
					</code>
				</pre>
			</li>
		</ol>
		<p class="work-sans light-text adjust-text">
			<strong>One more example for Post-increment and Pre-increment:</strong>
		</p>
		<pre class="adjust-text">
			<code class="language-java">
				{code[32]}
			</code>
		</pre>
		<p class="work-sans light-text adjust-text">
			<strong>Output:</strong>
		</p>
		<pre class="adjust-text">
			<code class="language-java">
				{code[33]}
			</code>
		</pre>
		<h3 class="questrial">Decrement</h3>
		<p class="work-sans light-text adjust-text">
            This is likewise a unary operator, meaning it only affects one operand. It's used to <strong>decrease</strong> an integer's value. It has two applications:
        </p>
		<ol class="work-sans light-text adjust-text">
			<li>
				<h4 class="questrial">Post-decrement</h4>
				<p class="work-sans light-text adjust-text">
					The value of the operand is decremented when it is placed after the variable name, but the previous values are retained temporarily until the execution of this statement, and they are updated before the execution of the next statement. Adding of <code>--</code> after the variable.
				</p>
				<p class="work-sans light-text adjust-text">
					Example:
				</p>
				<pre class="adjust-text">
					<code class="language-java">
						{code[34]}
					</code>
				</pre>
				<p class="work-sans light-text adjust-text">
					Output:
				</p>
				<pre class="adjust-text">
					<code class="language-java">
						{code[35]}
					</code>
				</pre>
			</li>
			<li>
				<h4 class="questrial">Pre-decrement</h4>
				<p class="work-sans light-text adjust-text">
					When the operand is placed before the variable name, the operand's value is immediately decremented. Adding of <code>-- before</code> the variable.
				</p>
				<p class="work-sans light-text adjust-text">
					Example:
				</p>
				<pre class="adjust-text">
					<code class="language-java">
						{code[36]}
					</code>
				</pre>
				<p class="work-sans light-text adjust-text">
					Output:
				</p>
				<pre class="adjust-text">
					<code class="language-java">
						{code[37]}
					</code>
				</pre>
			</li>
		</ol>
		<p class="work-sans light-text adjust-text">
			One more example for Post-decrement and Pre-decrement:
		</p>
		<pre class="adjust-text">
			<code class="language-java">
				{code[38]}
			</code>
		</pre>
		<p class="work-sans light-text adjust-text">
			Output:
		</p>
		<pre class="adjust-text">
			<code class="language-java">
				{code[39]}
			</code>
		</pre>
		
        <h2 class="questrial">Quick Test</h2>
        <!-- Question Card Content inside the pre tag-->
        <QuestionCard {...questionCardProps}>
            <pre class="question">
                int a = 5 + (3 * 5) / 5;
int b = ++a;
System.out.println(b);
            </pre>
        </QuestionCard>
        
        <div style="height: 10px;"></div>
        <div class="references">
            <h2 class="questrial">References</h2>
			<div class="questrial">
				<a href="https://www.geeksforgeeks.org/java-arithmetic-operators-with-examples/">GeeksForGeeks</a><br>
				<a href="https://tutorials.jenkov.com/java/math-operators-and-math-class.html#java-math-operators">Jenkov.com</a>
			</div>
        </div>
    </div>
    <div style="height: 3rem"></div>

    <!-- refer to the route list sent in GC -->
    <NavigationButton isFirstLesson={false} isLastLesson={false} prevLesson="commenting-in-java" nextLesson="operations-2"/>
    <div style="height: 3rem"></div>
</LessonTemplate>


<!-- Scope Styles -->
<style>
    .adjust-text {
        margin-left: 20px;
    }
</style>