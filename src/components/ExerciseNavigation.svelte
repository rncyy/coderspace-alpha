<!-- Data and Script -->
<script lang="ts">
    export let isFirstExercise: boolean;
    export let isLastExercise: boolean;
    export let prevExercise: string;
    export let nextExercise: string;
</script>

<!-- HTML -->
{#if isFirstExercise}
    <div class="d-flex justify-content-center">
        <a href="/#/exercises/{nextExercise}" class="btn btn-outline-info questrial no-dec">
            Next Exercise
        </a>
    </div>
{:else if isLastExercise}
    <div class="d-flex justify-content-center">
        <a href="/#/exercises/{prevExercise}" class="btn btn-outline-info questrial no-dec">
            Previous Exercise
        </a>
    </div>
{:else}
    <div class="row">
        <div class="col">
            <div class="d-flex justify-content-center">
                <a href="/#/exercises/{prevExercise}" class="btn btn-outline-info questrial no-dec">
                    Previous Exercise
                </a>
            </div>
        </div>
        <div class="col">
            <div class="d-flex justify-content-center">
                <a href="/#/exercises/{nextExercise}" class="btn btn-outline-info questrial no-dec">
                    Next Exercise
                </a>
            </div>
        </div>
    </div>
{/if}

<!-- Scope Styles -->
<style>

</style>