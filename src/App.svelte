<script>
  import svelteLogo from './assets/svelte.svg'
  import viteLogo from '/vite.svg'
  import Counter from './lib/Counter.svelte'
  import NiceKonto, {getTotal} from "./NiceKonto.svelte";

  const total = getTotal()
</script>

<main>
  <NiceKonto />
  <NiceKonto />
  <NiceKonto />

  <div class="card">
    <Counter />
  </div>

  <p>
    I have {total} items in my cart
    </p>

  <p class="read-the-docs">
    Click on the Vite and Svelte logos to learn more
  </p>
</main>
<svelte:head>
  <title>Svelte + Vite</title>
  <meta name="description" content="this is the svelte website I've been working on"/>
  </svelte:head>

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
