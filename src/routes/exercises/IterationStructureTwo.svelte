<!-- Data and Script -->
<script>
    import Navbar from "../../components/Navbar.svelte";
    import ExerciseContainer from "../../components/ExerciseContainer.svelte";
    let linkOne = "https://gist.github.com/rncyy/058b73a1d2958b216ebed8693624c46a";
    let linkTwo = "https://gist.github.com/rncyy/68cae4df50228faad6e2f3ac661a767e";
</script>

<!-- HTML -->
<Navbar/>
<ExerciseContainer lessonTitle="Iteration Structure (do...while)" linkOne={linkOne} linkTwo={linkTwo} prevExercise="iteration-structure-1" nextExercise="iteration-structure-3" isFirstExercise={false} isLastExercise={false}>
    <!-- question -->
    <div slot="question">
        Follow the specifications given for this exercise
    </div>
    <div slot="desc">
        <ol class="work-sans">
            <li>With the same program from the previous activity but change the class name to <code>DoWhileLoop</code></li>
            <li>Create a <code>do...while</code> loop that counts down from the integer variable value to zero</li>
            <li>If the number is an even number, print the words <code>Even Number!</code></li>
            <li>After counting down, print out <code>Done Counting Down!</code></li>
        </ol>
    </div>
</ExerciseContainer>
<!-- Scope Styles -->
<style>

</style>