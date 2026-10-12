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
        font-size: 1.7rem;
        font-family: AdventProVF;
        
         @media(prefers-reduced-motion: no-preference) {
            font-variation-settings: "wght" 900, "wdth" 110;
            transition: font-variation-settings 1.5s ease-in-out;
        }

        &:hover {
            font-variation-settings: "wght" 900, "wdth" 160;
        }

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