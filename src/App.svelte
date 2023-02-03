<script>
  import Logo from './assets/Icon.svg'

  const uData = {
    username: '',
    password: '',
  }

  function onSubmit(event) {
    event.preventDefault()
    fetch('', {
      method: 'POST',
      headers: {
        'Content-Type': 'application/json'
      },
      body: JSON.stringify({
        username: uData.username,
        password: uData.password,
      })
    })
    .then(response => response.json())
    .then(result => console.log(result))
  }
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
          <input type="text" id="username" name="username" bind:value={uData.username} placeholder="Username"/>
        </div>
        <div>
          <input type="password" id="password" name="password" bind:value={uData.password} placeholder="Password"/>
        </div>
        <button on:click="{onSubmit}">LOGIN</button>
    </form>
</main>

<style>
  .logo {
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
