<!-- Data and Script -->
<script>
    import Navbar from "../../components/Navbar.svelte";
    import ExerciseContainer from "../../components/ExerciseContainer.svelte";
    let linkOne = "https://gist.github.com/rncyy/c21083e500caa77f2d3c0b9ed7cfd8d5";
    let linkTwo = "https://gist.github.com/rncyy/5234071ccb2cd0e64a8e8e6306927eb6";
</script>

<!-- HTML -->
<Navbar/>
<ExerciseContainer lessonTitle="Variables in Java" linkOne={linkOne} linkTwo={linkTwo} nextExercise="commenting-in-java" isFirstExercise={true} isLastExercise={false}>
    <!-- question -->
    <div slot="question">
        Create a program with the following specifications
    </div>
    <div slot="desc">
        <ol class="work-sans">
            <li>Class name of <code>Variables</code></li>
            <li>
                Create 5 variables with the following types with logical variable names and assign a value
                <ul>
                    <li>String</li>
                    <li>Double</li>
                    <li>Integer</li>
                    <li>Character</li>
                    <li>Boolean</li>
                </ul>
            </li>
            <li>Print out all variables using <code>System.out.println();</code></li>
            <li>Change the value of the String, Character, and Integer variables</li>
            <li>Print out all variables once again</li>
        </ol>
    </div>
</ExerciseContainer>
<!-- Scope Styles -->
<style>

</style>