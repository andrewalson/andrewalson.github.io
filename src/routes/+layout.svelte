<script>

    // import { base } from "$app/paths";
    const linkedInUrl = "https://www.linkedin.com/in/andrewalson/";
  
  </script>

<nav>
    <a prefetch href="/">Home</a>
    <a href="/projects">Projects</a>
    <a href="/experience">Experience</a>
    <a href={linkedInUrl} target="_blank" rel="noopener noreferrer">Resume <span class="link">→</span></a>
</nav>

<slot /> 

<footer></footer>

<style>
    nav {
        background-color: orange;
        padding-top: .9rem;
        padding-bottom: 1.8rem;
    }
    nav a {
        float: left;
        text-decoration: none;
        width: 25%; /* Four equal-width links. If you have two links, use 50%, and 33.33% for three links, etc.. */
        text-align: center; /* If you want the text to be centered */
    }
    nav,
    footer {
        font-size: 0.8rem;
        letter-spacing: 0.1px;
        font-weight: bold;
    }

    :global(html) {
        --width: 700px;
        padding-left: max(1rem, calc(calc(100vw - var(--width)) / 2));
        padding-right: max(1rem, calc(calc(100vw - var(--width)) / 2));
    }

    /* main {
        margin-bottom: 5rem;
        margin-top: 5vw;
    } */
    
</style>