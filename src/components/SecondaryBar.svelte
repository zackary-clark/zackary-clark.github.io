<header>
    <ul class="nav-bar" id="secondary-bar">
        <li><a class="header-link text-link" href="#portfolio">Portfolio</a></li>
        <li><a class="header-link text-link" href="#hosting">Hosting</a></li>
        <li><a class="header-link text-link" href="#tracker">Tracker</a></li>
        <li><a class="header-link text-link" href="#snake-game">Snake</a></li>
    </ul>
</header>

<style>
    header {
        display: block;
        width: 100%;
        top: 3em;
        position: fixed;
    }

    ul {
        list-style-type: none;
        margin: 0;
        padding: 0;
        width: 100%;
        display: flex;
        align-items: center;
        box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
        background-color: var(--secondary);
        color: var(--fg0);
        height: 2em;
        top: 3em;
    }

    a:link {
        color: var(--fg0);
    }

    a:hover {
        color: var(--primary);
    }

    li > a {
        padding: 0 .5em;
        font-size: 1em;
    }
</style>
