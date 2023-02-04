<script>
    import svelteLogo from './assets/svelte.svg'
    import Counter from './lib/Counter.svelte'

    let name = "Azat"

    function toggleName() {
        if (name === "world") {
            name === "Svelte"
        } else {
            name = "world"
        }
    }
</script>

<main>

    <h1>Hello {name} from MDN!</h1>
    <button on:click={toggleName}>Toggle Name</button>

    <div class="card">
        <Counter/>
    </div>

    <p>
        Check out <a href="https://github.com/sveltejs/kit#readme" target="_blank" rel="noreferrer">SvelteKit</a>, the
        official Svelte app framework powered by Vite!
    </p>

    <p class="read-the-docs">
        Click on the Vite and Svelte logos to learn more
    </p>
</main>

<style>
    .logo {
        height: 6em;
        padding: 1.5em;
        will-change: filter;
        transition: filter 300ms;
    }

    .logo:hover {
        filter: drop-shadow(0 0 2em #646cffaa);
    }

    .logo.svelte:hover {
        filter: drop-shadow(0 0 2em #ff3e00aa);
    }

    .read-the-docs {
        color: #888;
    }
</style>
