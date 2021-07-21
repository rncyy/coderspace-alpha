<!-- Data and Script -->
<script>
    // this is for the name of the developer
    export let name;
    // this is for the name of the image file
    export let fileName;
    // this is for the socials
    export let facebook;
    export let twitter;
    export let instagram;
    
</script>

<!-- HTML -->
<div class="card border-info card-shadows card-bg" style="width: 18rem;">
    <img class="card-img-top" src="assets/{fileName}.jpg" alt="Developer">
    <div class="card-body">
        <h5 class="card-title questrial text-center">{name}</h5>
        <hr/>
        <p class="card-text desc work-sans text-justify">
            <slot/>
        </p>
    </div>
    <div class="card-footer border-info">
        <div class="d-flex justify-content-center">
            <div class="row">
                <div class="col-4">
                    <a target="_blank" href="https://twitter.com/{twitter}" class="btn btn-outline-info">
                        <img src="assets/twitter-logo.png" width="30" alt="Twitter Logo">
                    </a>
                </div>
                <div class="col-4">
                    <a target="_blank" href="https://facebook.com/{facebook}" class="btn btn-outline-info">
                        <img src="assets/facebook-logo.png" width="30" alt="Facebook Logo">
                    </a>
                </div>
                <div class="col-4">
                    <a target="_blank"  href="https://instagram.com/{instagram}" class="btn btn-outline-info">
                        <img src="assets/instagram-logo.png" width="30" alt="Instagram Logo">
                    </a>
                </div>
            </div>
        </div>
    </div>
</div>

<!-- Scope Styles -->
<style>
    .card-shadows {
        box-shadow: 0 0 2px #333333;
    }
    .card-bg {
        background-color: whitesmoke;
    }
</style>