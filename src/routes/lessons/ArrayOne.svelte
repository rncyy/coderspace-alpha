<!-- Data and Script -->
<!--suppress HtmlUnknownAnchorTarget -->
<script>
    import Navbar from "../../components/Navbar.svelte";
    import LessonTemplate from "../../components/LessonTemplate.svelte";
    import QuestionCard from "../../components/QuestionCard.svelte";
    import NavigationButton from "../../components/NavigationButton.svelte";

    let subtext = "Learn how Java handles arrays, a basic collection structure of data with the same data type.";
    let code = [
        "String[] studentName;\n" +
        "double[] studentGrade;",

        "String[] studentName = {\"Rence\", \"Hazel\", \"Gemarie\"};\n" +
        "double[] studentGrade = {90.25, 91.31, 90.50};",

        "String[] studentName = {\"Rence\", \"Hazel\", \"Gemarie\"};\n" +
        "System.out.println(studentName[0]);\n" +
        "// Outputs Rence",

        "double[] studentGrade = {90.25, 91.31, 90.50};\n" +
        "System.out.println(studentGrade[1]);\n// Outputs 91.31\n" +
        "studentGrade[1] = 94.10;\n" +
        "System.out.println(studentGrade[1]);\n// Outputs 94.10",

        "String[] ____ = {\"Shinichi\", \"Heiji\", \"Conan\"};"
    ];
    let questionCardProps = {
        lessonTitle: "Creating a new Array",
        questionTitle: "Create a new array with the name classmates",
        correctAnswer: "classmates"
    };
    let correctFeedback = "Nice work! You are ready for the next lesson!";
    let incorrectFeedback = "Revisit the requirement and try answering again";
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
<LessonTemplate lessonName="Arrays (Part 1)" imageName="array-1" subtext={subtext}>
    <div class="content">
        <h2 class="questrial">Arrays in Java (Part 1)</h2>
        <img src="https://d2h0cx97tjks2p.cloudfront.net/blogs/wp-content/uploads/sites/2/2018/02/Arrays-in-java-df.jpg" width="500" alt="java" class="mb-3 d-block mx-auto"/>
        <p class="work-sans light-text adjust-text">
            Arrays are used to store multiple data that are otherwise illogical to declare with different names.
        </p>
        <span class="work-sans light-text adjust-text">
            <strong>Practical Examples</strong>
        </span>
        <ol class="work-sans light-text adjust-text">
            <li>Students - If you are storing names of multiple students in a record, it would be illogical to name each of them <code>student1</code>, <code>student2</code>, <code>student3</code> and so on.</li>
            <li>Grades of students - Likewise if you are storing the grades of students, it would be impractical to separate the records with different names</li>
        </ol>
        <h3 class="questrial">Creating an array</h3>

        <p class="work-sans light-text adjust-text">
            To declare an array, define the variable type with <strong>square brackets</strong>
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[0]}
            </code>
        </pre>
        <p class="work-sans light-text adjust-text">
            We have now declared two variables each of which holds an array of strings and doubles. To insert values to it, we can use an array literal. We should place the values in a comma-separated list, inside curly braces as follows
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[1]}
            </code>
        </pre>
        <h3 class="questrial">Accessing the Elements inside an array</h3>
        <p class="work-sans light-text adjust-text">
            You can access the elements of the array by referring to its index number.
        </p>
        <p class="work-sans light-text adjust-text">
            The code below accesses the value of the first element in <code>studentName</code>
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[2]}
            </code>
        </pre>
        <div class="alert alert-primary d-flex align-items-center adjust-text" role="alert">
            <svg class="bi flex-shrink-0 me-2" width="24" height="24" role="img" aria-label="Info:"><use xlink:href="#info-fill"/></svg>
            <div class="work-sans light-text">
                Array indices start with 0 with 0 being the first element, 1 as the second, etc.
            </div>
        </div>
        <h3 class="questrial">Changing an element in the Array</h3>
        <p class="work-sans light-text adjust-text">
            To change an element inside an array, refer to the index number of the specific element you want to change and assign the new value to it.
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[3]}
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
                <a href="https://www.w3schools.com/java/java_arrays.asp">W3Schools - Java Arrays</a><br>
            </div>
        </div>
    </div>
    <div style="height: 3rem"></div>

    <!-- refer to the route list sent in GC -->
    <NavigationButton isFirstLesson={false} isLastLesson={false} prevLesson="iteration-structure-3" nextLesson="array-2"/>
    <div style="height: 3rem"></div>
</LessonTemplate>


<!-- Scope Styles -->
<style>
    .adjust-text {
        margin-left: 20px;
    }
</style>