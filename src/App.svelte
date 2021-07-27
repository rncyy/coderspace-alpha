<!-- Data and Script -->
<script lang="ts">
    import Router from 'svelte-spa-router';

    // pages
    import Home from './routes/Home.svelte';
    import About from './routes/About.svelte';
    import ContactUs from './routes/ContactUs.svelte';
    import Lessons from './routes/Lessons.svelte';
    import Exercises from './routes/Exercises.svelte';

    // lessons
    import HelloWorld from './routes/lessons/HelloWorld.svelte';
    import VariablesInJava from './routes/lessons/VariablesInJava.svelte';
    import CommentingInJava from './routes/lessons/CommentingInJava.svelte';
    import OperationsOne from './routes/lessons/OperationsOne.svelte';
    import OperationsTwo from './routes/lessons/OperationsTwo.svelte';
    import DecisionStructureOne from './routes/lessons/DecisionStructureOne.svelte';
    import DecisionStructureTwo from './routes/lessons/DecisionStructureTwo.svelte';
    import IterationStructureOne from './routes/lessons/IterationStructureOne.svelte';
    import IterationStructureTwo from './routes/lessons/IterationStructureTwo.svelte';
    import IterationStructureThree from './routes/lessons/IterationStructureThree.svelte';
    import ArrayOne from './routes/lessons/ArrayOne.svelte';
    import ArrayTwo from './routes/lessons/ArrayTwo.svelte';

    // exercises
    import VariablesInJavaEx from './routes/exercises/VariablesInJava.svelte';
    import CommentingInJavaEx from './routes/exercises/CommentingInJava.svelte';
    import OperationsOneEx from './routes/exercises/OperationsOne.svelte';
    import OperationsTwoEx from './routes/exercises/OperationsTwo.svelte';
    import DecisionStructureOneEx from './routes/exercises/DecisionStructureOne.svelte';
    import DecisionStructureTwoEx from './routes/exercises/DecisionStructureTwo.svelte';
    import IterationStructureOneEx from './routes/exercises/IterationStructureOne.svelte';
    import IterationStructureTwoEx from './routes/exercises/IterationStructureTwo.svelte';
    import IterationStructureThreeEx from './routes/exercises/IterationStructureThree.svelte';
    import ArrayOneEx from './routes/exercises/ArrayOne.svelte';
    import ArrayTwoEx from './routes/exercises/ArrayTwo.svelte';
</script>


<!-- HTML -->
<!-- ROUTER CONFIGURATIONS -->
<Router routes={{
    '/': Home,
    '/about': About,
    '/contact-us': ContactUs,
    '/lessons': Lessons,
    '/exercises': Exercises,
    // route for lessons
    '/lessons/hello-world': HelloWorld,
    '/lessons/variables-in-java': VariablesInJava,
    '/lessons/commenting-in-java': CommentingInJava,
    '/lessons/operations-1': OperationsOne,
    '/lessons/operations-2': OperationsTwo,
    '/lessons/decision-structure-1': DecisionStructureOne,
    '/lessons/decision-structure-2': DecisionStructureTwo,
    '/lessons/iteration-structure-1': IterationStructureOne,
    '/lessons/iteration-structure-2': IterationStructureTwo,
    '/lessons/iteration-structure-3': IterationStructureThree,
    '/lessons/array-1': ArrayOne,
    '/lessons/array-2': ArrayTwo,
    // route for the exercises
    '/exercises/variables-in-java': VariablesInJavaEx,
    '/exercises/commenting-in-java': CommentingInJavaEx,
    '/exercises/operations-1': OperationsOneEx,
    '/exercises/operations-2': OperationsTwoEx,
    '/exercises/decision-structure-1': DecisionStructureOneEx,
    '/exercises/decision-structure-2': DecisionStructureTwoEx,
    '/exercises/iteration-structure-1': IterationStructureOneEx,
    '/exercises/iteration-structure-2': IterationStructureTwoEx,
    '/exercises/iteration-structure-3': IterationStructureThreeEx,
    '/exercises/array-1': ArrayOneEx,
    '/exercises/array-2': ArrayTwoEx,
}} />

<!-- Scope Styles -->
<style>

</style>