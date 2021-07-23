<!-- Data and Script -->
<script>
    import Navbar from "../../components/Navbar.svelte";
    import ExerciseContainer from "../../components/ExerciseContainer.svelte";
    let linkOne = "";
    let linkTwo = "";
</script>

<!-- HTML -->
<Navbar/>
<ExerciseContainer lessonTitle="Decision Structure Two" linkOne={linkOne} linkTwo={linkTwo} prevExercise="decision-structure-1" nextExercise="iteration-structure-1" isFirstExercise={false} isLastExercise={false}>
    <!-- question -->
    <div slot="question">
        Follow the specifications given for this exercise
    </div>
    <div slot="desc">
        <ol class="work-sans">
            <li>Create a class with name <code>DecisionStructTwo</code></li>
            <li>Create a variable with the name <code>testValue</code> and assign the value 10</li>
            <li>Create a decision structured statement which prints if the number is either negative, positive, or zero using a <code>switch</code> statement</li>
        </ol>
    </div>
</ExerciseContainer>
<!-- Scope Styles -->
<style>

</style>