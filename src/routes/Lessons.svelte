<!-- Data and Script -->
<script>
    import LessonCard from "../components/LessonCard.svelte";
    import Navbar from "../components/Navbar.svelte";

</script>

<!-- HTML -->
<Navbar/>
<div class="d-flex justify-content-center mt-3">
    <div class="mb-2 mt-2">
        <div class="heading-text questrial text-center">
            <h1>
                Lessons and Tutorials <img src="assets/lesson.png" width="60" style="margin-bottom: 5px" alt="">
            </h1>
        </div>
    </div>
</div>
<div class="d-flex justify-content-center mt-3">
    <div class="row">
        <div class="col-4 mb-2">
            <LessonCard lessonName="Hello World with Java" lessonLink="hello-world" imageName="cmd">
                <p class="desc">
                    Let us start our Java Journey by writing the famous first program: "Hello World" in an online compiler called <a href="https://www.onlinegdb.com/online_java_compiler" target="_blank">OnlineGDB</a>!
                </p>
            </LessonCard>
        </div>
        <div class="col-4 mb-2">
            <LessonCard lessonName="Variables in Java" lessonLink="variables-in-java" imageName="variable">
                <p class="desc">
                    Learn about how Java take tabs on the data present inside a program. Look into the different types of data Java primitively supports!
                </p>
            </LessonCard>
        </div>
        <div class="col-4 mb-2">
            <LessonCard lessonLink="commenting-in-java" lessonName="Commenting in Java" imageName="comment">
                <p class="desc">
                    Learn the importance of adding comments in your programs, its practical uses, and its implications for your programs.
                </p>
            </LessonCard>
        </div>
    </div>
</div>
<div class="d-flex justify-content-center mt-3">
    <div class="row">
        <div class="col-6 mb-2">
            <LessonCard lessonLink="operations-1" lessonName="Operations in Java 1" imageName="plus" maxWidth="24.7rem">
                <p class="desc">
                    Check out how to perform operations in your data! This chapter includes mathematical operations and how some of the comparison operators work.
                </p>
            </LessonCard>
        </div>
        <div class="col-6 mb-2">
            <LessonCard lessonLink="operations-2" lessonName="Operations in Java 2" imageName="equals" maxWidth="24.7rem">
                <p class="desc">
                    Know the basics of assignment operators and logical operators in Java and be able to use them effectively in your programs, combined with other operators.
                </p>
            </LessonCard>
        </div>
    </div>
</div>
<div class="d-flex justify-content-center mt-3">
    <div class="row">
        <div class="col-6 mb-2">
            <LessonCard lessonLink="decision-structure-1" lessonName="Decision Structures 1" imageName="decision" maxWidth="24.7rem">
                <p class="desc">
                    Let your program make its own decision! Learn how programs make their decision using the decision structure: single way <code>if</code>, and the <code>if...else</code> structure
                </p>
            </LessonCard>
        </div>
        <div class="col-6 mb-2">
            <LessonCard lessonLink="decision-structure-2" lessonName="Decision Structures 2" imageName="decision" maxWidth="24.7rem">
                <p class="desc">
                    Let your program make its own decision! Learn how programs make their decision using the decision structure: nested <code>if...else</code> codes, and the <code>switch</code> statement.
                </p>
            </LessonCard>
        </div>
    </div>
</div>
<div class="d-flex justify-content-center mt-3">
    <div class="row">
        <div class="col-4 mb-2">
            <LessonCard lessonName="Iteration Structures 1" lessonLink="iteration-structure-1" imageName="loop-1">
                <p class="desc">
                    Learn how to perform repetitive operations using loops and iteration structures starting with the <code>while...</code> loop
                </p>
            </LessonCard>
        </div>
        <div class="col-4 mb-2">
            <LessonCard lessonName="Iteration Structures 2" lessonLink="iteration-structure-2" imageName="loop-2">
                <p class="desc">
                    Learn how to perform repetitive operations using loops and iteration structures by familiarizing yourself with the <code>do...while</code> loop
                </p>
            </LessonCard>
        </div>
        <div class="col-4 mb-2">
            <LessonCard lessonName="Iteration Structures 3" lessonLink="iteration-structure-3" imageName="loop-3">
                <p class="desc">
                    Learn how to perform repetitive operations using loops and iteration structures by compounding all iteration loops with the <code>for</code> loop
                </p>
            </LessonCard>
        </div>
    </div>
</div>
<div class="d-flex justify-content-center mt-3">
    <div class="row">
        <div class="col-6 mb-2">
            <LessonCard lessonLink="array-1" lessonName="Arrays 1" imageName="array-1" maxWidth="24.7rem">
                <p class="desc">
                    Check out your first data collection structure that stores multiple values of the same data type. Learn how to declare, and access data inside an array along with some tips when creating an array of your own
                </p>
            </LessonCard>
        </div>
        <div class="col-6 mb-2">
            <LessonCard lessonLink="array-2" lessonName="Arrays 2" imageName="array-2" maxWidth="24.7rem">
                <p class="desc">
                    Check out your first data collection structure that stores multiple values of the same data type. Learn how to loop over an array, and some useful methods to manipulate your arrays
                </p>
            </LessonCard>
        </div>
    </div>
</div>
<!-- Scope Styles -->
<style>

</style>