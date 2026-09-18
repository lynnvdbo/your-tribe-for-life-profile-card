<script>
    let {data} = $props()    
    let person = data.person[32];
</script>

<div class="kaart-container">
    <div class="buiten-rechthoek">       
        <div class="binnen-rechthoek">
            <div class="rechthoek-foto">
                <img class="image" src="{ person.avatar }" alt="{ person.name }" width="300" height="360">
            </div>
            <h1>{ person.name.split(' ')[0]}</h1> 
                <section class="info">    
                    <h2>Naam:</h2>
                    <p>{ person.name }</p>
                    <h2>Stad:</h2>
                    <p>{ person.residency }</p>
                    <h2>Bio:</h2>
                    <p>{ person.bio }</p>
                </section>
        </div>
    </div>

    <div class="zwart-vlak"></div>
</div>

<style>
    .kaart-container {
        position: relative; /*alles wat absolute is, mag zich binnen deze container positioneren*/
        width: 572px;
        height: 728px;
        margin: 5rem auto;
    }
    .zwart-vlak {
        position: absolute;
        inset: 0;
        width: 550px;
        height: 700px;
        background-color: var(--black);
        padding: 0.7rem;
        z-index: 10;

        animation: none;
        opacity: 0;
        @media(prefers-reduced-motion: no-preference) {
                animation: fadeOut 5s ease forwards;
            }
    }
    .buiten-rechthoek {
        position: absolute;
        inset: 0;
        padding: 0.7rem;
        width: 550px;
        height: 700px;
        background-color: var(--white);
        z-index: 1;
    }
    .binnen-rechthoek {
        display: grid;
        align-items: flex-start;
        width: 550px;
        height: 700px;
        background-color: var(--secondary-color);
    }
    .rechthoek-foto {
        width: fit-content;
        background-color: var(--white);
        padding: 1rem 1rem 1.5rem 1rem ;
        margin-top: 2rem;
        margin-right: 10rem;
        margin-left: 2rem;
        img {
            display: block;
            width: 300px;
            height: 360px;
            object-fit: cover; /* zorgt er voor dat de foto niet vervormd is */
        }
    }
    h1 {
        font-size: 11rem;
        font-family: Sirivennela;
        font-weight: 200;
        text-transform: uppercase;
        transform: rotate(-90deg);
        position: absolute;
        top: 40%;
        left: 56%;
        color: var(--black);
    } 
    .info {
        margin-left: 2rem;
        margin-block: 2rem;
        h2 {
            font-size: 1.1rem;
            text-transform: uppercase;
            font-family: boldonse, sans-serif;
        }   
        p {
            margin-bottom: 0.9rem;
        }
    }
    @keyframes fadeOut {
        from {
            opacity: 1;
        }

        to {
            opacity: 0;
        }
    }
</style>npm inat