<!-- Data and Script -->
<script>
    import Navbar from "../../components/Navbar.svelte";
    import LessonTemplate from "../../components/LessonTemplate.svelte";
    import QuestionCard from "../../components/QuestionCard.svelte";
    import NavigationButton from "../../components/NavigationButton.svelte";

    let subtext = "Let's begin our Java Journey by writing the famous first program: \"Hello World!\""
    let code = [
        "// HelloWorld.java\n" +
        "public class HelloWorld {\n" +
        "\tpublic static void main(String[] args) {\n" +
        "\t\tSystem.out.println(\"Hello World!\")\n" +
        "\t}\n" +
        "}",

        "// MainClass.java\n" +
        "public class MainClass {\n" +
        "\tpublic static void main(String[] args) {\n" +
        "\t\tSystem.out.println(\"Hello World!\")\n" +
        "\t}\n" +
        "}",

        "System.out.println(\"Hey There!\") \n//prints Hey There!\n" +
        "System.out.println(\"CoderSpace Alpha\") \n//prints CoderSpace Alpha\n" +
        "System.out.println(\"Java is the best!\") \n//prints Java is the best",

        "System.out.println() \n// prints what is inside the parenthesis",
    ];
    let questionCardProps = {
        lessonTitle: "Printing out text in the console in Java",
        questionTitle: "Fill in the blank to print out Java is Great",
        correctAnswer: "println"
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
<LessonTemplate lessonName="Hello World in Java" imageName="cmd" subtext={subtext}>
    <div class="content">
        <h2 class="questrial">What is Java?</h2>
        <img src="https://www.thoughtco.com/thmb/1XNPA2mDZJCuwBv8bgd5t8FCEHQ=/2310x0/filters:no_upscale():max_bytes(150000):strip_icc():format(webp)/what-is-java-5b4bda1cc9e77c0037171617.jpg" width="400" alt="java" class="mb-3 d-block mx-auto"/>
        <p class="work-sans light-text adjust-text">
            Java is an Object-Oriented Programming language developed by Sun Microsystems in 1995. A lot of applications and softwares is dependent on Java, and more of these applications are created everyday! Java is fast, secure, and reliable which makes it one of the programming languages preferred by many companies to build their projects on.
        </p>
        <p class="work-sans light-text adjust-text">
            Java is used to create Android Apps and develop a wide range of mobile Java applications. It is also used for big data analytics and scientific computing applications. Java is also used for programming some hardware devices.
        </p>
        <p class="work-sans light-text adjust-text">
            Though Java is quite verbose, meaning it is "wordy" and is quite a pain to type, it is actually one of the easy-to-use programming languages out there! Its multiplatforming capabilities allow you to write code once, and run it on almost any platform. Below is an example of a Java Program that prints out "Hello World!"
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[0]}
            </code>
        </pre>
        <p class="work-sans light-text adjust-text">
            Now that we know what Java is and its primary uses both in short-term, and its significance in the industry, let us learn the code above!
        </p>
        <p class="work-sans light-text adjust-text">
            Every individual Java file has a <code>public class ...</code>, and a <code>main()</code> method as seen below. As you may have noticed from the two code blocks above and below, the name of the class: <code>HelloWorld</code> and <code>MainClass</code> is the same as the Java file's name. Take note that the <strong>Class Name</strong> should be the same with the <strong>Java File Name</strong>
        </p>
        <h2 class="questrial">Hello World Program</h2>
        <p class="work-sans light-text adjust-text">
            We are now going to try to do a "Hello World" program using a method called <code>System.out.println()</code>
        </p>
        <pre>
            <code class="language-java">{code[1]}</code>
        </pre>
        <p class="work-sans light-text adjust-text">
            As mentioned earlier, an individual Java file consists of a <code>public class ...</code> and a <code>main()</code> method. For now, let us ignore those two concepts as we'll get back on them through the course of this tutorial. As you can see, inside those <code>public class</code> and <code>main()</code> method is a command called
        </p>
        <pre class="adjust-text"><code class="language-java">{code[3]}</code></pre>
        <p class="work-sans light-text adjust-text">
            <code>System.out.println()</code> is a very straightforward method to print text on the console. Follow the example below!
        </p>
        <div class="alert alert-primary d-flex align-items-center adjust-text" role="alert">
            <svg class="bi flex-shrink-0 me-2" width="24" height="24" role="img" aria-label="Info:"><use xlink:href="#info-fill"/></svg>
            <div class="work-sans light-text">
                For the next examples, we will omit the <code>public class ...</code> and <code>main()</code> portion since it will be redundant to put these when every single Java file is understood to have such code.
            </div>
        </div>
        <pre class="adjust-text">
            <code class="language-java">
                {code[2]}
            </code>
        </pre>
        <p class="work-sans light-text adjust-text">
            We can print almost all types of information by using the <code>System.out.println()</code> method. That's why it is a very handy method to know.
        </p>
        <h2 class="questrial">Quick Test</h2>

        <!-- Question Card Content inside the pre tag-->
        <QuestionCard {...questionCardProps}>
            <pre class="question">
                System.out._____("Java is Great");
            </pre>
        </QuestionCard>

        <div style="height: 10px;"></div>
        <div class="references">
            <h2 class="questrial">References</h2>
            <div class="questrial">
                <a href="https://www.guru99.com/java-platform.html">Guru99 - The Java Platform</a>
            </div>
        </div>
    </div>
    <div style="height: 3rem"></div>

    <!-- refer to the route list sent in GC -->
    <NavigationButton isFirstLesson={true} isLastLesson={false} nextLesson="variables-in-java"/>
    <div style="height: 3rem"></div>
</LessonTemplate>


<!-- Scope Styles -->
<style>
    .adjust-text {
        margin-left: 20px;
    }
</style>