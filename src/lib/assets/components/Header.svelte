<nav>
    <a href="https://github.com/lynnvdbo">Github</a>
    <a href="#">Portfolio</a>
    <a href="#">Contact</a>
</nav>

<style>

    @font-face {
        font-family: AdventProVF;
        src: url("/fonts/AdventPro-VF.ttf") format("truetype");
        font-weight: 100 900;
        font-stretch: 100% 200%;
    }
    nav {
        display: flex;
        gap: 1.5rem;
        position: fixed;
        top: 2rem;
        left: 3rem;
        z-index: 1000; 
        font-family: boldonse, sans-serif;

        a {
            text-decoration: none;
            color: var(--white);
            text-transform: uppercase;
            
            &:hover {
                text-decoration: underline;
                color: var(--secondary-color);
            }
        }
    }
</style>