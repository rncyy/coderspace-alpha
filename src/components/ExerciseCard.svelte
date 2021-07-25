<!--suppress ALL -->
<!-- Data and Logic -->
<script lang="ts">
    // for the file name of image
    export let imageName: string = "asset-about";
    // for the lesson name
    export let lessonName: string = "Lesson";
    // for the link of lesson (this is from routes)
    export let lessonLink: string = "hello-world";
    export let maxWidth: string = "16rem";
</script>

<!-- HTML -->
<a href="/#/exercises/{lessonLink}" class="no-dec">
    <div class="card" style="width: {maxWidth};">
        <div class="logo-bg d-flex">
            <img src="assets/{imageName}.png" class="card-img-top logo-width mx-auto mt-2 mb-2" alt="...">
        </div>
        <div class="card-body black no-dec mt-2">
            <h5 class="card-title text-center questrial no-dec">{lessonName}</h5>
            <p class="card-text desc text-center work-sans small-text no-dec">
                <slot/>
            </p>
        </div>
    </div>
</a>
<!-- Styling -->
<style>
    .logo-bg {
        background-color: whitesmoke;
    }
    .logo-width {
        width: 50px;
    }
    .black {
        color: black;
    }
    .no-dec {
        text-decoration: none;
    }
    .small-text {
        font-size: 15px;
    }
</style>