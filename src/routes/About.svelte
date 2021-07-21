<!-- Data and Script -->
<script>
    import Navbar from "../components/Navbar.svelte";
    import ProfileCard from "../components/ProfileCard.svelte";
    const hazelInfo = {
        name: "Hazel Anne Mejias",
        fileName: "hazel",
        facebook: "heyselnattt",
        twitter: "heyselnattt",
        instagram: "heyselnattt"
    }
    const gemInfo = {
        name: "Gemarie Magtangob",
        fileName: "gem",
        facebook: "dyimareeeeey",
        twitter: "krungsie",
        instagram: "gemawieee"
    }
    const renceInfo = {
        name: "Clarence Rhey Salaveria",
        fileName: "rence",
        facebook: "rncyy",
        twitter: "rncyy",
        instagram: "_eluxify"
    }
</script>

<!-- HTML -->
<Navbar/>
<div class="d-flex justify-content-center">
    <div class="mb-2 mt-2">
        <div class="heading-text questrial text-center">
            <h1>
                About the Developers <img src="assets/developer-about.png" width="60" alt="developer">
            </h1>
        </div>
        <div class="text-center questrial subtext">
            <p>
                We are CodeGrammeristz and we are the developers behind CoderSpace
            </p>
        </div>
        <div class="row">
            <div class="col-4">
                <ProfileCard {...renceInfo}>
                    <p class="desc">
                        I am a rhythm gamer and a Java enthusiast which is currently studying towards a career in the field of Information Technology. I play Arcaea, and chart songs in Malody in my free time. Proficiencies include Java, Python, and SvelteJS
                    </p>
                </ProfileCard>
            </div>
            <div class="col-4">
                <ProfileCard {...hazelInfo}>
                    <p class="desc">
                        I am into photography, editing photos and such. Sometimes I also love designing webpage and I also play online games such as CODM, etc. I am currently taking Information Technology at Pamantasan ng Lungsod ng Valenzuela.
                    </p>
                </ProfileCard>
            </div>
            <div class="col-4">
                <ProfileCard {...gemInfo}>
                    <p class="desc">
                        I am an avid KPop fan and also I really love watching KDrama. I love listening music and I'm currently studying in the field of Information Technology. I like programming in Java, structuring content in HTML and studying CSS
                    </p>
                </ProfileCard>
            </div>
        </div>
    </div>
</div>
<div class="d-flex justify-content-center mt-3 mb-3">
    <div class="mb-2 mt-2">
        <div style="height:30px"></div>
        <div class="heading-text questrial text-center">
            <h1>
                About the Project <img src="assets/notebook-about.png" width="60" alt="notebook">
            </h1>
        </div>
        <div class="questrial subtext d-flex justify-content-center align-content-center">
            <div class="container">
                <div class="row">
                    <div class="col-12">
                        <div class="container">
                            <div class="card text-center card-shadows card-bg">
                                <div class="card-body">
                                    <p class="card-text">
                                        We started this project mainly because it is one of our final requirements but it grew on us that this website has the potential to grow and help many people. One of the goals of this website is to provide concise learning materials while being able to interact with the user. We achieved this by using a question and answer approach and an interactive activity which allows you to fill-in-the-blanks of certain codes.
                                    </p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="row mt-3 mb-3">
                    <div class="col-6">
                        <div class="heading-text questrial text-center">
                            <h1>
                                Content Handling <img src="assets/pdf-about.png" width="60" alt="file">
                            </h1>
                            <div class="container">
                                <div class="card text-center card-shadows card-bg">
                                    <div class="card-body">
                                        <p class="card-text">
                                            The content in the learning materials posted and made available here are both proofread, and fact-checked to avoid any kinds of inconsistencies with the proper way to perform a task. With our goal to educate more people about Java, rest assured that no information that is not properly checked will go through and be made available to this website. If you do see any inconsistencies or errors, kindly
                                            <a target="_blank" href="/#/contact-us">Contact us</a> to get it resolved.
                                        </p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-6">
                        <div class="heading-text questrial text-center">
                            <h1>
                                Color Schemes <img src="assets/colorwheel-about.png" width="60" alt="colorwheel">
                            </h1>
                            <div class="container">
                                <div class="card text-center card-shadows card-bg">
                                    <div class="card-body">
                                        <p class="card-text">
                                            For this project, We have used the color scheme White, Cyan, with a hint of purple which is inspired by the color pallette used for our logo and other graphics found in this website. White is used to provide a clean and sleek interface comboed with a lively cyan and purple for our accent colors. We have also used the same color scheme with the Lesson pages, Quick Test page, and the Exercises Page. This ensures that the website is not just pure white.
                                        </p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div style="height:30px"></div>
                <div class="row mb-3 mt-3 text-center">
                    <div class="heading-text questrial text-center mt-2"></div>
                    <h1>
                        Attributions <img src="assets/guarantee.png" width="60" style="margin-bottom: 15px" alt="">
                    </h1>
                    <div class="col-4">
                        <div class="heading-text questrial text-center"></div>
                        <h1>
                            Frameworks <img src="assets/framework-about.png" width="60" alt="framework">
                        </h1>
                        <div class="container">
                            <div class="card text-center card-shadows card-bg">
                                <div class="card-body">
                                    <p class="card-text">
                                        CoderSpace Alpha was made possible by multiple development frameworks. One of them is <a target="_blank" href="https://svelte.dev">SvelteJS</a>, a JavaScript framework designed to work alongside HTML code. For our CSS, and some interactive elements, we have used
                                        <a target="_blank" href="https://getbootstrap.com">Bootstrap 5</a>. This provided us with page responsiveness and design with minimal coding.
                                    </p>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-4">
                        <div class="heading-text questrial text-center"></div>
                        <h1>
                            Services <img src="assets/software-about.png" width="60" alt="services">
                        </h1>
                        <div class="container">
                            <div class="card text-center card-shadows card-bg">
                                <div class="card-body">
                                    <p class="card-text">
                                        We used both the hosting services <a target="_blank" href="https://www.000webhost.com/">000webhost</a> and <a target="_blank" href="https://app.netlify.com/">Netlify</a>. Both of these hosting services features great capabilities. We also used
                                        <a target="_blank" href="https://formspree.io/">FormSpree</a> to establish a working static server. This allows us to gather responses without the need for an actual server. <a target="_blank" href="https://testmail.app/">Testmail.app</a> is used to test the forms by giving unlimited emails to test your form.
                                    </p>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-4">
                        <div class="heading-text questrial text-center"></div>
                        <h1>
                            Assets <img src="assets/asset-about.png" width="60" alt="assets">
                        </h1>
                        <div class="container">
                            <div class="card text-center card-shadows card-bg">
                                <div class="card-body">
                                    <p class="card-text">
                                        We have used assets from <a target="_blank" href="https://icons8.com">icons8</a> for the various graphics present in this website such as the icons, graphics, favicons, etc. In addition, We have used fonts from
                                        <a target="_blank" href="https://fonts.google.com">Google Fonts</a> to help provide suitable typography for our website. <a href="https://github.com/EmilTholin/svelte-routing" target="_blank">Svelte Routing</a> is a library which provided Routing or linking capabilities for our Svelte powered website.
                                    </p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>

<!-- Scope Styles -->
<style>
    .subtext {
        font-size: 24px;
    }
    .card-shadows {
        box-shadow: 0 0 3px #17a2b8;
    }
    .card-bg {
        background-color: whitesmoke;
    }
</style>