<script>
  let loggedIn = false;
    function login() {
        loggedIn = true;
    }
</script>

<button type="submit" on:click={login}>
  LOGIN
</button>
