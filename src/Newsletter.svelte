
<style>
    section {
        position: relative;
        z-index: 15;
        width: 100% ;
        background-color: #f3fffc;
    }

    .block {
        
        max-width: 800px;
        margin: 0px auto;
        padding: 50px 100px 60px;
    }

    label {
        margin: 0 0 60px;
        font-family: 'battlefin', sans-serif;
	    font-weight: 400;
        font-style: normal;
        font-size: 1.3rem ;
        line-height: 1.2;
        cursor: pointer ;
    }

    p {
        font-size: 1.5rem ;
        margin:0;
    }

    .para {
        font-size:1.5rem ;
    }

    h2 {
        padding-top:20px;
        font-size: 3.2rem;
        line-height: 1;
        text-shadow:1px 1px 2px #86fadb;
    }

    h2, p {text-align: center ;}

    input, input:focus {
        height: 30px ;
        width: 100% ;
        border: 1px solid #278e73;
        cursor: pointer ;
        margin: 0 0 32px;
        color: #278e73;
        text-align:center;
        font-size: 1.7rem;
        padding: 8px 0;
    }

    button {
        background: #ff22aa;
        color:white;
        padding: 20px 40px;
        border:none;
        font-size:1.5rem;
        box-shadow: 1px 1px 3px rgba(128, 128, 128, 0.425);
        transition: all 0.25s ease-out;
        cursor: pointer;
        border-radius:10px;
        position: relative;
        left:50%;
        transform: translate(-50%,0%);
    }

    button:focus, button:hover {
        background: #86fadb;
        color:#ff22aa;
        box-shadow:none;
        border-radius:50px;
    }

    @media only screen and (max-width:725px) {
        .block {
        position: relative ;
        max-width: 100%;
        margin: 60px 20px 60px;
        padding: 0 20px;
    }

        h2 {
            font-size:2.1rem;
            padding-right:20px;
            text-align:left;
        }
        p {
            text-align: left;
            padding-right:20px;
        }
    }

    #Register {padding:20px;}
    
</style>

<section>
    <div class="block">
        <div id="Register" class="regBump"></div>
        <h2 class="title">Vous voulez devenir un foileux ?</h2>
        <p class="para">Veuillez remplir le formulaire ci-dessous.<br>Un agent vous contactera dans les prochaines 24 heures.</p>
        <br><br>
        <form name="FoilContactForm" method="POST" Content-Type="application/x-www-form-urlencoded" netlify action="/about">
            <input type="hidden" name="form-name" value="FoilContactForm" />
            
            <label for="name"><p>Nom et prénom</p></label>
                <input type="text" id="name" name="clientNames" placeholder="" required >
            
            <label for="phone"><p>Numéro de téléphone</p></label>
                <input type="tel" id="phone" name="clientPhone" placeholder="" required >
            
            <label for="email"><p>Adresse courriel</p></label>
                <input type="email" id="email" name="clientEmail"  required/>
            
            <button type="submit">INSCRIVEZ-VOUS</button>
        </form>
    </div>
</section>