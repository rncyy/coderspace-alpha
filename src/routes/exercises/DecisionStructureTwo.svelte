<!-- Data and Script -->
<script>
    import Navbar from "../../components/Navbar.svelte";
    import ExerciseContainer from "../../components/ExerciseContainer.svelte";
    let linkOne = "https://gist.github.com/rncyy/8b34370a1b850dc7f59a192bd2a6ef6c";
    let linkTwo = "https://gist.github.com/rncyy/e27fccf082ef3a6366324de4061b43bc";
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
            <li>Create a variable with the name <code>testValue</code> and assign any value from 1 to 7</li>
            <li>Create a decision structured statement which prints the corresponding day with the number. (1-Monday, ... 7-Sunday)</li>
            <li>If the value is not 1 to 7, print out <code>Invalid Day</code></li>
        </ol>
    </div>
</ExerciseContainer>
<!-- Scope Styles -->
<style>

</style>