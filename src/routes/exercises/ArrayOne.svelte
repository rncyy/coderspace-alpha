<!-- Data and Script -->
<script>
    import Navbar from "../../components/Navbar.svelte";
    import ExerciseContainer from "../../components/ExerciseContainer.svelte";
    let linkOne = "https://gist.github.com/rncyy/d5a3c9bf118462d08e703226592251cc";
    let linkTwo = "https://gist.github.com/rncyy/8fe1191d12158e7e798156a8b02f5185";
</script>

<!-- HTML -->
<Navbar/>
<ExerciseContainer lessonTitle="Arrays One" linkOne={linkOne} linkTwo={linkTwo} prevExercise="iteration-structure-3" nextExercise="array-2" isFirstExercise={false} isLastExercise={false}>
    <!-- question -->
    <div slot="question">
        Follow the specifications given for this exercise
    </div>
    <div slot="desc">
        <ol class="work-sans">
            <li>Create a class with name <code>ArrayOne</code></li>
            <li>Create an array with the name <code>cars</code> and initialize it with any value you like (minimum 5 elements)</li>
            <li>Create another array that contains integers and initialize it with any value you like (minimum 5 elements)</li>
            <li>Change the value of the following: <code>cars[3]</code> and the second element of your integer array</li>
        </ol>
    </div>
</ExerciseContainer>
<!-- Scope Styles -->
<style>

</style>