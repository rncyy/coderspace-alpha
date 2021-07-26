<!-- Data and Script -->
<script>
    import QuickTestAnswerField from "./QuickTestAnswerField.svelte";
    export let score;
    export let correctAnswer;
    let answerInput;
    export let questionTitle;
    export let lessonTitle;
    export let correctFeedback;
    export let incorrectFeedback;
</script>

<!-- HTML -->
<div class="card">
    <div class="card-header questrial text-center">
        {lessonTitle}
    </div>
    <div class="card-body">
        <h5 class="card-title questrial text-center">{questionTitle}</h5>
        <pre class="card-text question">
            <code class="language-java"><slot/></code>
        </pre>
        <div class="answer-field">
            <QuickTestAnswerField score={score} bind:textField={answerInput} answer={correctAnswer} correctFeedback={correctFeedback} incorrectFeedback={incorrectFeedback}/>
        </div>
    </div>
</div>

<!-- Scope Styles -->
<style>

</style>