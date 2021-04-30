<script>
  import { Link } from "svelte-routing";
  const name = "User";
  const apiUrl = API_URL;
</script>

<main>
  <Link to="/other">Go to Other</Link>
  <h1>Hello {name}! Api URL is {apiUrl}</h1>
  <p>
    Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn
    how to build Svelte apps.
  </p>
</main>

<style lang="scss">
  h1 {
    color: $primary;
    text-transform: uppercase;
  }
</style>
