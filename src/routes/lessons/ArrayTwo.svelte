<!-- Data and Script -->
<!--suppress HtmlUnknownAnchorTarget -->
<script>
    import Navbar from "../../components/Navbar.svelte";
    import LessonTemplate from "../../components/LessonTemplate.svelte";
    import QuestionCard from "../../components/QuestionCard.svelte";
    import NavigationButton from "../../components/NavigationButton.svelte";

    let subtext = "Learn the basic methods of managing your array more easily and learn how to loop over your arrays.";
    let code = [
        "String[] studentName = {\"Rence\", \"Hazel\", \"Gemarie\"};\n" +
        "int[] numbers = {9, 5, 6, 4, 2};\n" +
        "System.out.println(studentName.length); // 3\n" +
        "System.out.println(numbers.length); // 5\n",

        "String[] studentName = {\"Rence\", \"Hazel\", \"Gemarie\"};\n" +
        "for (int i < 1; i <= studentName.length; i++) {\n" +
        "\tSystem.out.print(studentName[i] + \" \");\n" +
        "}\n// Outputs Rence Hazel Gemarie",

        "String[] studentName = {\"Rence\", \"Hazel\", \"Gemarie\"};\n" +
        "for (String name: studentName) {\n" +
        "\tSystem.out.print(name + \" \");\n" +
        "}\n// Outputs Rence Hazel Gemarie",

        "double[] studentGrade = {90.25, 91.31, 90.50};\n" +
        "double result = 0.0;\n" +
        "double average = 0.0;\n" +
        "for (double grade: studentGrade) {\n" +
        "\tresult += _____;\n" +
        "}\n" +
        "average = average/studentGrade.length;\n" +
        "System.out.println(average);"
    ];
    let questionCardProps = {
        lessonTitle: "Operating with Arrays",
        questionTitle: "Complete the program to compute the average of the array: studentGrade",
        correctAnswer: "grade"
    };
    let correctFeedback = "Congratulations! You have completed the available lessons on CoderSpace!";
    let incorrectFeedback = "Try looking at the problem once more and try again.";
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
<LessonTemplate lessonName="Arrays (Part 2)" imageName="array-2" subtext={subtext}>
    <div class="content">
        <h2 class="questrial">Arrays in Java (Part 2)</h2>
        <img src="https://d2h0cx97tjks2p.cloudfront.net/blogs/wp-content/uploads/sites/2/2018/02/Arrays-in-java-df.jpg" width="700" alt="java" class="mb-3 d-block mx-auto"/>
        <h3 class="questrial"><code>length</code> attibute</h3>
        <p class="work-sans light-text adjust-text">
            Knowing the number of elements inside your array is particularly useful in looping over your array to perform operations on every element of the array. This can be achieved by the <code>.length</code> attribute of arrays.
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[0]}
            </code>
        </pre>
        <h3 class="questrial">Looping over an array (Thru index)</h3>
        <p class="work-sans light-text adjust-text">
            Arrays are particularly useful if you have multiple data for a variable. If you can store many instances of a data, it is only logical that we should access these data using a for loop with the length of the loop.
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[1]}
            </code>
        </pre>
        <h3 class="questrial">Looping over an array (Thru enhanced for loop)</h3>
        <p class="work-sans light-text adjust-text">
            You can use similar for loops to manage different arrays. In some instances, you can also use an enhanced for loop to perform operations with the elements of your array. For instance, check the following code.
        </p>
        <pre class="adjust-text">
            <code class="language-java">
                {code[2]}
            </code>
        </pre>
        <p class="work-sans light-text adjust-text">
            This enhanced for loop just takes each String element inside <code>studentName</code> and prints it. This type of loop makes it easier to deal with some arrays as this loop allows you to iterate by elements, and not by index.
        </p>
        <h2 class="questrial">Quick Test</h2>
        <!-- Question Card Content inside the pre tag-->
        <QuestionCard {...questionCardProps} correctFeedback={correctFeedback} incorrectFeedback={incorrectFeedback}>
            <pre class="question">
                {code[3]}
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
    <NavigationButton isFirstLesson={false} isLastLesson={true} prevLesson="iteration-structure-3"/>
    <div style="height: 3rem"></div>
</LessonTemplate>


<!-- Scope Styles -->
<style>
    .adjust-text {
        margin-left: 20px;
    }
</style>