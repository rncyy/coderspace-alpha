<!-- Data and Script -->
<script>
    import Navbar from "../../components/Navbar.svelte";
    import ExerciseContainer from "../../components/ExerciseContainer.svelte";
    let linkOne = "https://gist.github.com/rncyy/fb1c9c1d71cbcce1c0a17a32ed2e323e";
    let linkTwo = "https://gist.github.com/rncyy/403188f6c026bf53f883c7656f470390";
</script>

<!-- HTML -->
<Navbar/>
<ExerciseContainer lessonTitle="Iteration Structure (for loop)" linkOne={linkOne} linkTwo={linkTwo} prevExercise="iteration-structure-2" nextExercise="array-1" isFirstExercise={false} isLastExercise={false}>
    <!-- question -->
    <div slot="question">
        Follow the specifications given for this exercise
    </div>
    <div slot="desc">
        <ol class="work-sans">
            <li>Create a class with name <code>ForLooping</code></li>
            <li>Using the <code>for</code> loop, print out the numbers from -10 to 10</li>
        </ol>
    </div>
</ExerciseContainer>
<!-- Scope Styles -->
<style>

</style>