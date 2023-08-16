<script>
  import '../../global.css';
  import Title from '$lib/title.svelte';
</script>

<header>
  <Title />
  <div class='links'>
    <a href='/'>Home</a>
    <a href='/about'>About</a>
    <a href='/reviews'>Reviews</a>
  </div>
</header>
<main>
  <slot></slot>
</main>
<footer>
  <p>Copyright 2023 Casual Gamer Blog</p>
</footer>

<style>
  header {
    display: flex;
    justify-content: center;
  }
  main {
    max-width: 960px;
    margin: 20px auto;
  }
  footer {
    text-align: center;
  }
  .links {
    margin-left: auto;
  }
  a {
    margin-left: 10px;
  }
</style>
