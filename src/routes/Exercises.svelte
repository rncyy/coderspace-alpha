<!-- Data and Script -->
<script>
    import Navbar from "../components/Navbar.svelte";
    import ExerciseCard from "../components/ExerciseCard.svelte";

</script>

<!-- HTML -->
<Navbar/>
<div class="d-flex justify-content-center mt-3">
    <div class="mb-2 mt-2">
        <div class="heading-text questrial text-center">
            <h1>
                Exercises and Machine Problems <img src="assets/lesson.png" width="60" style="margin-bottom: 5px" alt="">
            </h1>
        </div>
    </div>
</div>
<div class="d-flex justify-content-center mt-3">
    <div class="row">
        <div class="col-6 mb-2">
            <ExerciseCard lessonName="Variables in Java" lessonLink="variables-in-java" imageName="variable" maxWidth="24.7rem">
                <p class="desc">
                    Try out your knowledge with variables in Java! Declare, modify, and print out your variable!
                </p>
            </ExerciseCard>
        </div>
        <div class="col-6 mb-2">
            <ExerciseCard lessonLink="commenting-in-java" lessonName="Commenting in Java" imageName="comment" maxWidth="24.7rem">
                <p class="desc">
                    Try out your knowledge with comments in Java! Create multiple comments to describe your program!
                </p>
            </ExerciseCard>
        </div>
    </div>
</div>
<div class="d-flex justify-content-center mt-3">
    <div class="row">
        <div class="col-6 mb-2">
            <ExerciseCard lessonLink="operations-1" lessonName="Operations in Java 1" imageName="plus" maxWidth="24.7rem">
                <p class="desc">
                    Perform simple operations with variables, and apply it to a formal exercise!
                </p>
            </ExerciseCard>
        </div>
        <div class="col-6 mb-2">
            <ExerciseCard lessonLink="operations-2" lessonName="Operations in Java 2" imageName="equals" maxWidth="24.7rem">
                <p class="desc">
                    Strengthen your understanding with a machine problem that focuses on shorthand assignment operators!
                </p>
            </ExerciseCard>
        </div>
    </div>
</div>
<div class="d-flex justify-content-center mt-3">
    <div class="row">
        <div class="col-6 mb-2">
            <ExerciseCard lessonLink="decision-structure-1" lessonName="Decision Structures 1" imageName="decision" maxWidth="24.7rem">
                <p class="desc">
                    Are you ready to let your program decide for you? Try out this machine exercise to more strengthen your knowledge.
                </p>
            </ExerciseCard>
        </div>
        <div class="col-6 mb-2">
            <ExerciseCard lessonLink="decision-structure-2" lessonName="Decision Structures 2" imageName="decision" maxWidth="24.7rem">
                <p class="desc">
                    Let's kick it up a notch! Solidify the foundation of your new knowledge by using nested conditionals!
                </p>
            </ExerciseCard>
        </div>
    </div>
</div>
<div class="d-flex justify-content-center mt-3">
    <div class="row">
        <div class="col-4 mb-2">
            <ExerciseCard lessonName="Iteration Structures 1" lessonLink="iteration-structure-1" imageName="loop-1">
                <p class="desc">
                    Loop over and start with a warm up exercise involving the <code>while</code> loop!
                </p>
            </ExerciseCard>
        </div>
        <div class="col-4 mb-2">
            <ExerciseCard lessonName="Iteration Structures 2" lessonLink="iteration-structure-2" imageName="loop-2">
                <p class="desc">
                    Try your knowledge about the <code>do...while</code> loop by a practice exercise!
                </p>
            </ExerciseCard>
        </div>
        <div class="col-4 mb-2">
            <ExerciseCard lessonName="Iteration Structures 3" lessonLink="iteration-structure-3" imageName="loop-3">
                <p class="desc">
                    Learn how to perform repetitive operations using loops and iteration structures by compounding all iteration loops with the <code>for</code> loop
                </p>
            </ExerciseCard>
        </div>
    </div>
</div>
<div class="d-flex justify-content-center mt-3">
    <div class="row">
        <div class="col-6 mb-2">
            <ExerciseCard lessonLink="array-1" lessonName="Arrays 1" imageName="array-1" maxWidth="24.7rem">
                <p class="desc">
                    Check out your first data collection structure that stores multiple values of the same data type. Learn how to declare, and access data inside an array along with some tips when creating an array of your own
                </p>
            </ExerciseCard>
        </div>
        <div class="col-6 mb-2">
            <ExerciseCard lessonLink="array-2" lessonName="Arrays 2" imageName="array-2" maxWidth="24.7rem">
                <p class="desc">
                    Check out your first data collection structure that stores multiple values of the same data type. Learn how to loop over an array, and some useful methods to manipulate your arrays
                </p>
            </ExerciseCard>
        </div>
    </div>
</div>
<!-- Scope Styles -->
<style>

</style>