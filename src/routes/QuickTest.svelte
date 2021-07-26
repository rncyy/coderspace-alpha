<!-- Data and Script -->
<script>
    import Navbar from "../components/Navbar.svelte";
    import QuickTestCard from "../components/QuickTestCard.svelte";
    // should be no more than 5
    let score = 0;
    let questionAnswer = {
        "questions": [
            "__________________(\"Hello World!\");",

            "System.out.println" +
            "int prodId = 12345;\n" +
            "String prodName = \"Flat Tops\";\n" +
            "_____ prodPrice = 15.75;",


        ],
        "answers": [
            "System.out.println",
            "double",

        ],
        "questionTitles": [
            "Fill in the blanks to print out \"Hello World\"",

        ]
    }
    let rand = Math.floor((Math.random() * 15) + 1);
    let questionCardProps = {
        lessonTitle: "Lets do the Quick Test!",
        questionTitle: rand,
        correctAnswer: questionAnswer.answers[rand-1],
    }
</script>

<!-- HTML -->
<Navbar/>
<div class="d-flex justify-content-center align-content-center">
    <div class="vertical-center">
        <QuickTestCard {...questionCardProps} score={score}>
            <pre className="question">
                {questionAnswer.questions[rand-1]}
            </pre>
        </QuickTestCard>
    </div>
</div>
<!-- Scope Styles -->
<style>
    .vertical-center {
        margin: 0;
        position: fixed;
        top: 50%;
        -ms-transform: translateY(-50%);
        transform: translateY(-50%);
    }
</style>