<script>
</script>

<style>

    .back {
        background-color: #f3fffc;
        padding: 0px 0 0px;
        margin-top:-100px;
        position: relative;
        z-index: 15;
    }

    section {
        position: relative;
        max-width: 800px;
        margin: 100px auto 0px;
    }

    .resp-container {
        position: relative;
        overflow: hidden;
        padding-top: 56.25%; /* This is 9th / 16th */
    }

    .resp-iframe {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        border: 0;
    }

    .cov {
        position: absolute;
        left:0;
        top:0;
        z-index: 115;
        background: rgba(189, 189, 189, 0);
        width:100%;
        height:100%;
    }

    @media only screen and (max-width:825px) {
        .cov {
            display:none;
        }
        h2 {
            margin-top:40px;
        }
    }
</style>

<div class="back">
    <section>
        <div class="resp-container">
            <div class="cov"></div>
            <iframe title="video showing the beach of Cayo Santa Maria"
                    class="resp-iframe"
                    src="https://www.youtube.com/embed/N6RdFH_6a1Q?controls=0&amp;start=7&end=72;&loop=1&playlist=N6RdFH_6a1Q&autoplay=1&mute=1" 
                    frameborder="0" 
                    allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture">
            </iframe>
        </div>
        <!-- <div class="fallback"></div> -->
    </section>
</div>