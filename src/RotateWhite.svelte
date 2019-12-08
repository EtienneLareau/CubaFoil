<style>
    
    
    p { font-family: bicyclette, sans-serif; 
            font-style: normal;
            text-shadow: 1px 1px 10px rgb(18, 97, 74); }



    @media only screen and (max-width:700px){

        p { font-size:1.3rem;
            line-height:1.3; }
    }
    /**/

    img {
        width:200px;
        margin-bottom:10px;
    }

    @keyframes rotating
	{
	from
		{
		transform: rotate(0deg);
		-o-transform: rotate(0deg);
		-ms-transform: rotate(0deg);
		-moz-transform: rotate(0deg);
		-webkit-transform: rotate(0deg);
		}
	to
		{
		transform: rotate(360deg);
		-o-transform: rotate(360deg);
		-ms-transform: rotate(360deg);
		-moz-transform: rotate(360deg);
		-webkit-transform: rotate(360deg);
		}
	}
    @-webkit-keyframes rotating
	{
	from
		{
		transform: rotate(0deg);
		-webkit-transform: rotate(0deg);
		}
	to
		{
		transform: rotate(360deg);
		-webkit-transform: rotate(360deg);
		}
	}
    
    .rotating
	{
	-webkit-animation: rotating 8s linear infinite;
	-moz-animation: rotating 8s linear infinite;
	-ms-animation: rotating 8s linear infinite;
	-o-animation: rotating 8s linear infinite;
	animation: rotating 8s linear infinite;
	}

    img {
        width:200px;
        position:fixed;
        z-index: 11;
        right:10px;
        bottom:10px;
    }
    
    .mid-text {
        position:fixed;
        z-index: 11;
        right:57px;
        bottom:50px;
        text-align: center;
        color: white;
        font-size:1.7rem;
        text-shadow: none;
    }

    @media only screen and (max-width:825px){
        img {
            bottom:50px;
            position: absolute;
        }

        .mid-text {
            bottom:90px;
            position: absolute;
        }
    }

    /* .hold {
        position: fixed;
        right:57px;
        bottom:50px;
    } */
</style>

<div class="hold">
<p class="mid-text">Prochain<br>voyage</p>
<img class="rotating" src="/images/Circle_dates3.png" alt="Les dates du voyage dédié Foil">
</div>