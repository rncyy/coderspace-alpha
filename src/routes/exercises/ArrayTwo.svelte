<!-- Data and Script -->
<script>
    import Navbar from "../../components/Navbar.svelte";
    import ExerciseContainer from "../../components/ExerciseContainer.svelte";
    let linkOne = "https://gist.github.com/rncyy/f4123f914ceb74987b832b68759edf3c";
    let linkTwo = "https://gist.github.com/rncyy/3deace4b53b459d59ed3c00fd05be430";
</script>

<!-- HTML -->
<Navbar/>
<ExerciseContainer lessonTitle="Arrays Two" linkOne={linkOne} linkTwo={linkTwo} prevExercise="array-1" isFirstExercise={false} isLastExercise={true}>
    <!-- question -->
    <div slot="question">
        Follow the specifications given for this exercise
    </div>
    <div slot="desc">
        <ol class="work-sans">
            <li>Using your created arrays in the previous activity: loop over your arrays to print them out individually</li>
            <li><code>cars[]</code> elements should be printed out using enhanced for loop</li>
            <li>Your integer array should be printed out through looping over the index</li>
        </ol>
    </div>
</ExerciseContainer>
<!-- Scope Styles -->
<style>

</style>