<script>

    import { base } from "$app/paths";
  
  </script>

<nav>
    <a prefetch href="/">Nav bar</a>
</nav>

<slot /> 

<footer>Footer</footer>

<style>
    nav {
        background: rgba(0, 0, 1, 2);
        padding-top: 1rem;
        padding-bottom: 1rem;
    }
    nav,
    footer {
        text-transform: uppercase;
        font-size: 0.7rem;
        letter-spacing: 0.1px;
        font-weight: 500;
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