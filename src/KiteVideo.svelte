<script>

</script>

<style>

    .back {
        background-color: #f3fffc;
        padding: 0px 0 0px;
        margin-top:-100px;
    }

    h2 {
        font-size:3.2rem;
        text-shadow: 1px 1px 3px #86fadb;
        padding:20px 0 0;
        margin:0;
    }

    section {
        position: relative;
        max-width: 800px;
        margin: 0px auto;
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
            font-size: 1.9rem;
            text-align: center;
        }
    }
</style>

<div class="back">
    <section>
        <h2>Le Spot</h2>
        <div class="resp-container">
            <div class="cov"></div>
            <iframe title="video showing the beach of Cayo Santa Maria"
                    class="resp-iframe"
                    src="https://www.youtube.com/embed/Jd2KnrbSPT0?controls=0&amp;start=7&end=72;&loop=1&playlist=Jd2KnrbSPT0&autoplay=1&mute=1" 
                    frameborder="0" 
                    allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture">
            </iframe>
        </div>
        <!-- <div class="fallback"></div> -->
    </section>
</div>