<!-- Data and Script -->
<script>
    import AnswerField from "./AnswerField.svelte";
    export let correctAnswer;
    let answerInput;
    export let questionTitle;
    export let lessonTitle;
    export let correctFeedback;
    export let incorrectFeedback;
</script>

<!-- HTML -->
<div class="card card-bg card-shadows">
    <div class="card-header questrial text-center">
        {lessonTitle}
    </div>
    <div class="card-body">
        <h5 class="card-title questrial text-center">{questionTitle}</h5>
        <pre class="card-text question">
            <code class="language-java"><slot/></code>
        </pre>
        <div class="answer-field">
            <AnswerField bind:textField={answerInput} answer={correctAnswer} correctFeedback={correctFeedback} incorrectFeedback={incorrectFeedback}/>
        </div>
    </div>
</div>

<!-- Scope Styles -->
<style>
    .card-shadows {
        box-shadow: 0 0 3px #17a2b8;
    }
    .card-bg {
        background-color: whitesmoke;
    }
</style>