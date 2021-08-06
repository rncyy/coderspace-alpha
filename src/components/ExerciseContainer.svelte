<!-- Data and Script -->
<script>
    import ExerciseNavigation from "./ExerciseNavigation.svelte";
    export let isLastExercise;
    export let isFirstExercise;
    export let nextExercise;
    export let prevExercise;
    export let lessonTitle;
    export let linkOne;
    export let linkTwo;
</script>

<!-- HTML -->
<div class="d-flex align-items-center justify-content-center">
    <div class="vertical-center card-bg card-shadows">
        <div class="card " style="width: 50rem;">
            <div class="card-header questrial d-inline-flex justify-content-center">
                <span class="fnt-9">{lessonTitle}</span>
            </div>
            <div class="card-body light-text work-sans">
                <div class="question questrial">
                    <slot name="question"/>
                </div>
                <div class="work-sans">
                    <slot name="desc"/>
                </div>
            </div>
        </div>
        <div class="row mt-3">
            <div class="col d-inline-flex justify-content-start">
                <a href="{linkOne}" target="_blank" class="questrial btn btn-outline-info">
                    Example solution 1
                </a>
            </div>
            <div class="col d-inline-flex justify-content-end">
                <a href="{linkTwo}" target="_blank" class="questrial btn btn-outline-info">
                    Example solution 2
                </a>
            </div>
        </div>
        <div class="row mt-3">
            <ExerciseNavigation isFirstExercise={isFirstExercise} isLastExercise={isLastExercise} nextExercise={nextExercise} prevExercise={prevExercise}/>
        </div>
    </div>
</div>


<!-- Styling -->
<style>
    .vertical-center {
        margin: 0;
        position: fixed;
        top: 50%;
        -ms-transform: translateY(-50%);
        transform: translateY(-50%);
    }

    .question {
        font-size: 18pt;
    }

    .fnt-9 {
        font-size: 20pt;
    }
    .card-shadows {
        box-shadow: 0 0 3px #17a2b8;
    }
    .card-bg {
        background-color: whitesmoke;
    }
</style>