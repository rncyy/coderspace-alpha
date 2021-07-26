<!-- Data and Script -->
<script>
    export let answer = "hello";
    export let textField;
    export let correctFeedback = "Congratulations! You got the correct answer!";
    export let incorrectFeedback = "You almost got it! Try revisiting the topic then try again";
    export let score
    let state = {
        isCorrect: false,
        isClicked: false
    }
    function checkAnswer() {
        state.isCorrect = textField===answer;
    }
    function clickButton() {
        state.isClicked = true;
    }
    function addScore() {
        if (textField===answer) {
            score+=1;
        }
    }
</script>

<!-- HTML -->
<div class="d-flex justify-content-center">
    <div class="row">
        <div class="col mx-auto">
            <input class="questrial" type="text" bind:value={textField}>
        </div>
        <div class="col mx-auto">
            <button on:click={checkAnswer} on:click={clickButton} on:click={addScore} class="questrial">Check Answer</button>
        </div>
    </div>
</div>


{#if state.isClicked}
    {#if state.isCorrect}
        <div class="answer text-center questrial">
            {correctFeedback} <br>
            <strong>Score is: {score}</strong>
        </div>
    {:else}
        <div class="incorrect text-center questrial">
            {incorrectFeedback}
        </div>
    {/if}
{/if}


<!-- Scope Styles -->
<style>
    .answer {
        color: #449300;
    }
    .incorrect {
        color: red;
    }
</style>