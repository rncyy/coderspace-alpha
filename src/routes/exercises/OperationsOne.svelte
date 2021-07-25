<!-- Data and Script -->
<script>
    import Navbar from "../../components/Navbar.svelte";
    import ExerciseContainer from "../../components/ExerciseContainer.svelte";
    let linkOne = "https://gist.github.com/rncyy/260f02c72eae19b3a34b8463f022370c";
    let linkTwo = "https://gist.github.com/rncyy/ce8f6cb9944dbb7a2b3f5c036c44c171";
</script>

<!-- HTML -->
<Navbar/>
<ExerciseContainer lessonTitle="Operations in Java 1" linkOne={linkOne} linkTwo={linkTwo} prevExercise="commenting-in-java" nextExercise="operations-2" isFirstExercise={false} isLastExercise={false}>
    <!-- question -->
    <div slot="question">
        Create a program with the specified requirements
    </div>
    <div slot="desc">
        <ol class="work-sans">
            <li>Create a class with name <code>OperationsOne</code></li>
            <li>Create two <code>double</code> variables named <code>gradeOne</code> and <code>gradeTwo</code></li>
            <li>Assign any values for the variables</li>
            <li>Perform addition, subtraction, multiplication, and division and print the results</li>
            <li>Only two variables may be declared and used</li>
        </ol>
    </div>
</ExerciseContainer>
<!-- Scope Styles -->
<style>

</style>