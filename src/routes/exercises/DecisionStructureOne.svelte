<!-- Data and Script -->
<script>
    import Navbar from "../../components/Navbar.svelte";
    import ExerciseContainer from "../../components/ExerciseContainer.svelte";
    let linkOne = "";
    let linkTwo = "";
</script>

<!-- HTML -->
<Navbar/>
<ExerciseContainer lessonTitle="Decision Structure One" linkOne={linkOne} linkTwo={linkTwo} prevExercise="operations-2" nextExercise="decision-structure-2" isFirstExercise={false} isLastExercise={false}>
    <!-- question -->
    <div slot="question">
        Follow the specifications given for this exercise
    </div>
    <div slot="desc">
        <ol class="work-sans">
            <li>Create a class with name <code>DecisionStruct</code></li>
            <li>Create a variable with the name <code>testValue</code> and assign the value 10</li>
            <li>Create a decision structured statement which prints if the number is either negative, positive, or zero using <code>if...else...</code></li>
        </ol>
    </div>
</ExerciseContainer>
<!-- Scope Styles -->
<style>

</style>