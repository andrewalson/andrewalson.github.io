<script>

    // import { base } from "$app/paths";
  
  </script>

<nav>
    <a prefetch href="/">Home</a>
    <a href="/projects">Projects</a>
    <a href="/pbc">PBC</a>
    <a href="/turing">Turing</a>
    <a href="/linkedin">LinkedIn</a>
    <a href="/github">GitHub</a>
</nav>

<slot /> 

<footer>Footer</footer>

<style>
    nav {
        background-color: orange;
        padding-top: .9rem;
        padding-bottom: 1.65rem;
    }
    nav a {
        float: left;
        text-decoration: none;
        width: 16.66%; /* Four equal-width links. If you have two links, use 50%, and 33.33% for three links, etc.. */
        text-align: center; /* If you want the text to be centered */
    }
    nav,
    footer {
        text-transform: uppercase;
        font-size: 0.7rem;
        letter-spacing: 0.1px;
        font-weight: bold;
    }

    :global(html) {
        --width: 700px;
        padding-left: max(1rem, calc(calc(100vw - var(--width)) / 2));
        padding-right: max(1rem, calc(calc(100vw - var(--width)) / 2));
    }

    main {
        margin-bottom: 5rem;
        margin-top: 5vw;
    }
    
</style>