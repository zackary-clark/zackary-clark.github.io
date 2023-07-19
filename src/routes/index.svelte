<svelte:head>
    <title>Zack's Portfolio</title>
</svelte:head>

<div id="main">
    <div id="headshot" class="main-container">
        <img src="./headshot.jpeg"  alt="headshot" width="256" height="256" />
        <h1>Zack Clark</h1>
    </div>
    <div class="main-container">
        <p>
            Welcome to my portfolio. It's where I show off my hobby projects, and <s>trick</s> convince people that I should be hired.
        </p>
        <p>
            I'm a former Air Force Officer and current Full Stack Software Engineer building PWAs and leading dev teams since 2018.
        </p>
        <p>
            My favorite environment is one where strong opinions are loosely held and radical honesty is the status quo.
        </p>
    </div>
</div>

<style>
    #main {
        padding: 1em;
        margin-top: 3em;
        display: flex;
        column-gap: 1em;
    }

    @media (max-width: 600px) {
        #main {
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }
    }

    h1 {
        margin: 0.25em;
    }

    .main-container {
        height: fit-content;
        width: fit-content;
    }

    .main-container > p {
        margin-bottom: 1em;
        margin-top: 0;
    }

    #headshot {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }
</style>
