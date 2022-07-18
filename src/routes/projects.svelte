<script>
    import Fa from "svelte-fa";
    import { faArrowUpRightFromSquare } from "@fortawesome/free-solid-svg-icons";
    import SecondaryBar from "../components/SecondaryBar.svelte";
</script>

<svelte:head>
    <title>Projects</title>
</svelte:head>

<SecondaryBar />
<div id="main">
    <div id="portfolio">
        <h1>Portfolio</h1>
        <p>
            This portfolio is written with SvelteKit. Why? Entirely because I wanted an excuse to use Svelte.
        </p>
        <p>
            The "right" tool for such a static page is almost certainly vanilla HTML and CSS, but what nerd can pass up a chance to use something new and interesting?
        </p>
    </div>
    <div id="hosting">
        <h1>Hosting</h1>
        <p>
            A Raspberry Pi based Kubernetes cluster hosts all my projects.
        </p>
        <p>
            It's more expensive, less scalable, and (probably) less secure than hosting on something like AWS.
            But none of those typically important hosting considerations were a factor, <i>learning</i> was.
            And building my own cluster from the ground up did make me learn. A lot.
            About Linux servers, K8s, Docker, networking, and more.
        </p>
        <h3>
            Tools/Frameworks in use
        </h3>
        <ul>
            <li>Kubernetes - Container Orchestration</li>
            <li>Docker - Container Runtime & Build</li>
            <li>Flannel CNI - Inter-node Network Fabric</li>
            <li>MetalLB - Load Balancing</li>
            <li>NGINX Ingress - Ingress (Exposing Services Outside Cluster)</li>
            <li>TrueNAS - Persistent Off-Cluster Storage</li>
            <li>NFS Subdir External Provisioner - Dynamic Persistent Volume Provisioner</li>
            <li>Kubegres - K8s Operator for PostgreSQL Instances</li>
            <li>Duck DNS - Free Dynamic DNS</li>
            <li>*upcoming* KeyCloak - Authentication & Authorization</li>
            <li>*upcoming* Let's Encrypt - Real SSL Cert(s)</li>
        </ul>
    </div>
    <div id="tracker">
        <h1>
            <a href="http://zackary-clark.duckdns.org/strongman-tracker/" target="_blank" rel="noopener noreferrer">
                Strongman Tracker <Fa icon={faArrowUpRightFromSquare} />
            </a>
        </h1>
        <p>
            This project has been in progress, off and on, since 2018.
            It started because I actually wanted (and still want) a workout tracking app to fill a niche that I haven't yet found a tool for.
        </p>
        <p>
            Over the years, I've added almost no features.
        </p>
        <p>
            This is due to heavily prioritizing learning, so my time has mostly gone toward migrations -
            meant to teach me frameworks and platforms I needed in my day job.
        </p>
        <p>
            It's moved from Heroku & GitHub Pages to my own K8s cluster. It's moved from MySQL to MongoDB to PostgreSQL. It's migrated from Java/Spring, to Express/Node, to Apollo Server. It was my first exposure to <i>both</i> Enzyme and React Testing Library.
            I've learned a ton. I've implemented almost no features. And I think that's mostly ok. The only downside is I <i>still</i> don't have a workout tracker that fills my needs.
        </p>
    </div>
</div>

<style>
    #main {
        padding: 1em;
        margin-top: 5em;
    }

    h1 {
        color: var(--primary);
    }

    h1 > a:link {
        color: var(--primary);
    }

    h1 > a:visited {
        color: var(--primary);
    }
</style>