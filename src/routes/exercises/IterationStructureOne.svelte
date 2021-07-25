<!-- Data and Script -->
<script>
    import Navbar from "../../components/Navbar.svelte";
    import ExerciseContainer from "../../components/ExerciseContainer.svelte";
    let linkOne = "https://gist.github.com/rncyy/4dda83583640c09efd6fd757c5d69708";
    let linkTwo = "https://gist.github.com/rncyy/7fa7ccf5a931d29aac13b11875f86791";
</script>

<!-- HTML -->
<Navbar/>
<ExerciseContainer lessonTitle="Iteration Structure (while...)" linkOne={linkOne} linkTwo={linkTwo} prevExercise="decision-structure-2" nextExercise="iteration-structure-2" isFirstExercise={false} isLastExercise={false}>
    <!-- question -->
    <div slot="question">
        Follow the specifications given for this exercise
    </div>
    <div slot="desc">
        <ol class="work-sans">
            <li>Create a class with name <code>WhileLoop</code></li>
            <li>Create a variable that contains an integer and assign it any value</li>
            <li>Create a <code>while...</code> loop that counts down from the integer variable value to zero</li>
            <li>After counting down, print out <code>Done Counting Down!</code></li>
        </ol>
    </div>
</ExerciseContainer>
<!-- Scope Styles -->
<style>

</style>