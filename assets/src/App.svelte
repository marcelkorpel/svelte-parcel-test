<script lang="ts">
    import Nested from "./Nested.svelte";

    export let name;

    function foo() {
        alert('foo');
    }
</script>

<main>
    <h1>Hello {name}!</h1>
    <p class="world">Visit the <a href="https://svelte.dev/tutorial" on:click={foo}>Svelte tutorial</a> to <span class="red">learn</span> how to build Svelte apps.</p>
<Nested/>
</main>

<style>
    main {
        text-align: center;
        padding: 1em;
        max-width: 240px;
        margin: 0 auto;
    }

    h1 {
        color: #ff3e00;
        text-transform: uppercase;
        font-size: 4em;
        font-weight: 100;
    }

    @media (min-width: 640px) {
        main {
            max-width: none;
        }
    }

    .red {
        color: green;
    }
</style>
