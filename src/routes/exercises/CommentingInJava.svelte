<!-- Data and Script -->
<script>
    import Navbar from "../../components/Navbar.svelte";
    import ExerciseContainer from "../../components/ExerciseContainer.svelte";
    let linkOne = "";
    let linkTwo = "";
</script>

<!-- HTML -->
<Navbar/>
<ExerciseContainer lessonTitle="Commenting in Java" linkOne={linkOne} linkTwo={linkTwo} prevExercise="variables-in-java" nextExercise="operations-1" isFirstExercise={false} isLastExercise={false}>
    <!-- question -->
    <div slot="question">
        Follow the specifications given for this exercise
    </div>
    <div slot="desc">
        <ol class="work-sans">
            <li>Add comments in your previously coded exercise</li>
            <li>Add as many comments as you need</li>
            <li>Use any of the comment types you have learned.</li>
        </ol>
    </div>
</ExerciseContainer>
<!-- Scope Styles -->
<style>

</style>