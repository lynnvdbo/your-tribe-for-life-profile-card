<script>
    import {zoekstatus} from '$lib/search.svelte.js';
    let {data} = $props()    
    let person = data.person[32];
</script>

<div class="kaart-container">
    <div class="buiten-rechthoek">       
        <div class="binnen-rechthoek">
            <div class="rechthoek-foto">
                <img class="image" src="{ person.avatar }" alt="{ person.name }" width="300" height="360">
            </div>
                <section class="info">
                    <h1>{ person.name.split(' ')[0]}</h1>    
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

<nav>
    <a href="https://github.com/lynnvdbo">
        <h3>Github</h3>
    </a>
    <a href="#">
        <h3>Portfolio</h3>
    </a>
    <a href="#">
        <h3>Contact</h3>
    </a>
</nav>

