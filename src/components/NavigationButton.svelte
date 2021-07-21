<!-- Data and Script -->
<script lang="ts">
    export let isFirstLesson: boolean;
    export let isLastLesson: boolean;
    export let prevLesson: string;
    export let nextLesson: string;
</script>

<!-- HTML -->
{#if isFirstLesson}
    <div class="d-flex justify-content-end">
        <a href="/#/lessons/{nextLesson}" class="btn btn-outline-info">
            Next Lesson
        </a>
    </div>
{:else if isLastLesson}
    <div class="d-flex justify-content-start">
        <a href="/#/lessons/{prevLesson}" class="btn btn-outline-info">
            Previous Lesson
        </a>
    </div>
{:else}
    <div class="row">
        <div class="col">
            <div class="d-flex justify-content-start">
                <a href="/#/lessons/{prevLesson}" class="btn btn-outline-info questrial no-dec">
                    Previous Lesson
                </a>
            </div>
        </div>
        <div class="col">
            <div class="d-flex justify-content-end">
                <a href="/#/lessons/{nextLesson}" class="btn btn-outline-info questrial no-dec">
                    Next Lesson
                </a>
            </div>
        </div>
    </div>
{/if}

<!-- Scope Styles -->
<style>

</style>