<header>
    <ul class="nav-bar" id="secondary-bar">
        <li><a class="header-link text-link" href="#portfolio">Portfolio</a></li>
        <li><a class="header-link text-link" href="#hosting">Hosting</a></li>
        <li><a class="header-link text-link" href="#tracker">Tracker</a></li>
    </ul>
</header>
<div id="main">
    <div id="hosting">
        <h1>Hosting</h1>
        <p>I made a Raspberry Pi 4 cluster which I'm hosting my projects on. Is it more performant than hosting on AWS
           or Azure? Probably not. Is it cheaper? Definitely not. Is it more secure? I imagine not, but I tried! Does it
           offer flexibility that I could not otherwise get? Sure, but I'm not really <i>doing</i> anything with that
           flexibility. But it did make me learn more about Linux servers, K8s, Docker, networking, etc. than hosting on
           a cloud provider. And isn't learning the real purpose of personal projects anyway? </p>
    </div>
    <div id="portfolio">
        <h1>Portfolio</h1>
    </div>
    <div id="tracker">
        <h1>Strongman Tracker</h1>
    </div>
</div>

<style>
    header {
        display: block;
        width: 100%;
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

    #main {
        padding: 1em;
    }
</style>