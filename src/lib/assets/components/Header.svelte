<nav>
    <a href="https://github.com/lynnvdbo">Github</a>
    <a href="#">Portfolio</a>
    <a href="#">Contact</a>
</nav>

<style>
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