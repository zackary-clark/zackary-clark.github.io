<script>
    import Fa from "svelte-fa";
    import { faLinkedin, faGithub } from "@fortawesome/free-brands-svg-icons";
    import { faTerminal, faEnvelope } from "@fortawesome/free-solid-svg-icons";
</script>

<header>
    <ul>
        <li class="header-padding"></li>
        <li id="header-logo">
            <a class="header-link" href="/">
                <Fa size="2x" icon={faTerminal} />
            </a>
        </li>
        <li>
            <a class="header-link text-link" href="/projects">
                Projects
            </a>
        </li>
        <li>
            <a class="header-link" href="https://www.linkedin.com/in/zackary-clark/">
                <Fa size="1.5x" icon={faLinkedin} />
            </a>
        </li>
        <li>
            <a class="header-link" href="mailto:zack@zclark.dev">
                <Fa size="1.5x" icon={faEnvelope} />
            </a>
        </li>
        <li>
            <a class="header-link" href="https://github.com/zackary-clark">
                <Fa size="1.5x" icon={faGithub} />
            </a>
        </li>
        <li class="header-padding"></li>
    </ul>
</header>

<style>
    header {
        display: block;
        width: 100%;
        top: 0;
        position: fixed;
    }

    ul {
        list-style-type: none;
        margin: 0;
        padding: 0;
        height: 3em;
        width: 100%;
        top: 0;
        display: flex;
        align-items: center;
        box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
        background-color: var(--primary);
    }

    .header-padding {
        width: 1em;
    }

    #header-logo {
        margin-right: auto;
        padding-left: .5em;
    }

    .header-link {
        padding: 0 .5em;
    }

    .text-link {
        font-size: 1em;
    }
</style>
