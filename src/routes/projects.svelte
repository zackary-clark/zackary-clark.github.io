<svelte:head>
    <title>Projects</title>
</svelte:head>

<header>
    <ul class="nav-bar" id="secondary-bar">
        <li><a class="header-link text-link" href="#portfolio">Portfolio</a></li>
        <li><a class="header-link text-link" href="#hosting">Hosting</a></li>
        <li><a class="header-link text-link" href="#tracker">Tracker</a></li>
    </ul>
</header>
<div id="main">
    <div id="portfolio">
        <h1>Portfolio</h1>
        <p>This portfolio is written with SvelteKit. Why? Because I kept reading about Svelte, and wanted an excuse to use it. I think the "right" tool for such a page is vanilla HTML and CSS, but what nerd can pass up a chance to use an interesting new technology?</p>
    </div>
    <div id="hosting">
        <h1>Hosting</h1>
        <p>I made a Raspberry Pi 4 cluster which I'm hosting my projects on. Is it more performant than hosting on AWS
           or Azure? Probably not. Is it cheaper? Definitely not. Is it more secure? I imagine not, but I tried! Does it
           offer flexibility that I could not otherwise get? Sure, but I'm not really <i>doing</i> anything with that
           flexibility. But it did make me learn more about Linux servers, K8s, Docker, networking, etc. than hosting on
           a cloud provider. And isn't learning the real purpose of personal projects anyway? </p>
    </div>
    <div id="tracker">
        <h1>Strongman Tracker</h1>
        <p>
            This is my real baby. This project has been worked on, more or less, since 2018. It started because I actually wanted a workout tracking app to fill a niche that I haven't yet found a tool for.
            Over the years, I've added almost no features. Mostly because my time has instead gone to migrations meant to learn core frameworks and platforms to help in my day-to-day job.
            That's meant this thing has gone through a ton of changes that add up to almost no differences if you look at it. It's moved from Heroku to my own Raspberry Pi cluster. It's moved from MySQL to MongoDB to PostGreSQL. It's migrated from Java/Spring, to Express/Node, to Apollo Server. It was my first exposure to <i>both</i> Enzyme and React Testing Library.
            I've learned a ton. I've implemented almost no features. And I think that's mostly ok. The only downside is I <i>still</i> don't have a workout tracker that fills my needs.
        </p>
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