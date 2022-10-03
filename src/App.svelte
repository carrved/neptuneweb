<script>
  import svelteLogo from './assets/svelte.svg';
  import Counter from './lib/Counter.svelte';

  const openSellix = () => {
    window.open("https://pornhub.com");
  }

  const openShowcase = () => {
    window.open("https://www.youtube.com/watch?v=LZ3khexIxhw");
  }

</script>

<main>
  <h1 class="rainbow">neptune</h1>
  <hr />
  <button class="button" on:click={openSellix}>purchase</button>
  <button class="button" on:click={openShowcase}>showcase</button>
</main>

<style>
  * {
    font-family: monospace;
  }
  .button {
    background-color: transparent;
  }
  .rainbow {
    text-align: center;
    font-family: monospace;
    letter-spacing: -1px;
    animation: colorRotate 6s linear 0s infinite;
  }

  @keyframes colorRotate {
    from {
      color: #6666ff;
    }
    10% {
      color: #0099ff;
    }
    50% {
      color: #6666ff;
    }
    75% {
      color: #0099ff;
    }
    100% {
      color: #6666ff;
    }
  }
</style>
