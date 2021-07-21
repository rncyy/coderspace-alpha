<!-- Data and Script -->
<script lang="ts">
    import Router from 'svelte-spa-router';
    import Home from './routes/Home.svelte';
    import About from './routes/About.svelte';
    import ContactUs from './routes/ContactUs.svelte';
    import Lessons from './routes/Lessons.svelte';
    import QuickTest from './routes/QuickTest.svelte';
    import Exercises from './routes/Exercises.svelte';
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

</script>


<!-- HTML -->
<!-- ROUTER CONFIGURATIONS -->
<Router routes={{
    '/': Home,
    '/about': About,
    '/contact-us': ContactUs,
    '/lessons': Lessons,
    '/quicktest': QuickTest,
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
    '/exercises/variables-in-java': VariablesInJava,
    '/exercises/commenting-in-java': CommentingInJava,
    '/exercises/operations-1': OperationsOne,
    '/exercises/operations-2': OperationsTwo,
    '/exercises/decision-structure-1': DecisionStructureOne,
    '/exercises/decision-structure-2': DecisionStructureTwo,
    '/exercises/iteration-structure-1': IterationStructureOne,
    '/exercises/iteration-structure-2': IterationStructureTwo,
    '/exercises/iteration-structure-3': IterationStructureThree,
    '/exercises/array-1': ArrayOne,
    '/exercises/array-2': ArrayTwo,
}} />

<!-- Scope Styles -->
<style>

</style>