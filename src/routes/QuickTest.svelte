<!-- Data and Script -->
<script>
    import Navbar from "../components/Navbar.svelte";
    import QuestionCard from "../components/QuestionCard.svelte";
    // should be no more than 5
    let questionCounter = 0;
    let questionAnswer = {
        "questions": [

        ],
        "answers": [
            1,2,3,4,5,6,7,8,9,10,11,12,13,14,15
        ]
    }
    let rand = Math.floor((Math.random() * 15) + 1);
</script>

<!-- HTML -->
<Navbar/>
<!--<QuestionCard lessonTitle="Quick Test Question!" correctAnswer={questionAnswer[1][rand] - 1}>-->
<!--    <pre class="question">-->
<!--        {questionAnswer[1][rand]}-->
<!--    </pre>-->
<!--</QuestionCard>-->
<!-- Scope Styles -->
<style>

</style>