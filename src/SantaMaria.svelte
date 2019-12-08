    
    
    

<style>
    article {
        max-width: 800px;
        width: 80% ;
        margin: 40px auto 0;
        padding: 60px 0 0px;
    }

    p {
        font-size: 1.7rem ;
        font-family: bicyclette, sans-serif;
        font-weight: 400;
        font-style: normal;
        padding: 5px;
    }

    h2 {
        font-family: 'feltro-texture-3', sans-serif;
        font-size: 4.2rem;
        
        text-shadow: 2px 2px 5px #86fadb;
    }

    img {
        width:80px;
        margin:20px 0 -10px;
        float:left;
        padding: 0px 15px;
    }


    @media only screen and (min-width:766px) and (max-width:1115px) {
      
        p {
           font-family: bicyclette, sans-serif;
            font-weight: 400;
            font-style: normal;
            font-size: 1.7rem ;
            padding: 0 1em;
        }
    
        h2 {
        font-family: 'feltro-texture-3', sans-serif;
        font-size: 3.2rem;
        padding: 0 20px;
        text-shadow: 2px 2px 5px #86fadb;
        }
    }


    @media only screen and (max-width:765px) {
        article {
            width:100%;
        }
     
        p {
            font-family: bicyclette, sans-serif;
            font-weight: 400;
            font-style: normal;
            padding: 0 1em;
            font-size:1.3rem;
        }
      
        h2 {
        font-family: 'feltro-texture-3', sans-serif;
        font-size: 2.7rem;
        padding: 0 20px 10px;
        text-align: center;
        text-shadow: 2px 2px 5px #86fadb;
        }
    }
    /* //////////////// */

    .start {
        margin-top:-40px;
        background-image: url('/images/coursLight.jpeg');
        background-position: center;
        background-repeat: no-repeat ;
        background-size: cover;
        position: relative;
        z-index: 15;
    }

    .fade {
        position: relative;
        z-index: 100;
        background: rgba(255, 255, 255, 0.603);
        width:100%;
        height:100%;
    }

    h3 {
        font-size:3.2rem;
        text-shadow: 1px 1px 3px #86fadb;
        padding:20px 0 0;
        margin:0;
    }

    section {
        position: relative;
        max-width: 800px;
        margin: 0px auto 0px;
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
         h3 {
             font-size: 1.9rem;
             text-align: center;
            margin-top:0px;
        }
    }

</style>

<div class="start">
    <div class="fade">
        <article>
            <h2>Cayo Santa Maria</h2>
            <p>Situé à une quinzaine de kilomètres de Cayo Guillermo, 
                Cayo Santa Maria vous offre les mêmes conditions de vent,
                 d'eau chaude turquoise et d'espace, le tout sur fond de 
                 sable blanc, sans roche.</p>
            
            <p>Un terrain de jeu exceptionnel à découvrir: Une immense zone 
                de " flat water " près du parc National, parfait pour les apprentis 
                et les intermédiaires voulant pratiquer des manoeuvres. L'endroit idéal 
                pour pratiquer l'hydrofoil en toute sécurité.</p>
            
            <p>À deux pas de votre chambre, la plage du Valentin 
             Club Perla Blanca est un endroit paradisiaque et unique, 
            l'un des meilleurs SPOTS des Caraïbes.</p>
        </article>
        
        <section>
            <h3>La plage</h3>
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
</div>
