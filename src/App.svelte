<script>
  import Logo from './assets/Icon.svg'
  import Submit from './lib/Submit.svelte'
</script>

<main>s
  <div id="head">
    <a href="https://bezpecnost.ssps.cz" rel="noreferrer">
      <img src={Logo} class="logo" alt="Logo" />
    </a>
    </div>
    <h1>Login Page</h1>
    <form>
        <div>
          <input type="Username" placeholder="Username"/>
        </div>
        <div>
          <input type="Password" placeholder="Password"/>
        </div>
        <Submit/>
    </form>
</main>

<style>
  .logo {
    color: red;
    height: 7em;
    padding: 1em;
    will-change: filter;
    transition: filter 300ms;
  }
  .logo:hover {
    filter: drop-shadow(0 0 2em #646cff);
  }
  .logo:hover {
    filter: drop-shadow(0 0 2em #646cff);
  }
</style>
