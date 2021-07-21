<!--suppress ALL -->
<!-- Data and Script -->
<script>
    export let lessonName = " ";
    export let imageName = " ";
    export let subtext = " ";
</script>

<!-- HTML -->
<div class="d-flex justify-content-center">
    <div class="mb-2 mt-2">
        <div class="heading-text questrial text-center">
            <h1>
                {lessonName} <img src="assets/{imageName}.png" width="60" style="margin-bottom: 5px" alt="">
            </h1>
        </div>
        <div class="text-center questrial">
            <p class="subtitle">{subtext}</p>
        </div>
    </div>
</div>
<div class="container w-50 content">
    <slot/>
</div>

<!-- Scope Styles -->
<style>
    .subtitle {
        font-size: 20px;
    }
</style>