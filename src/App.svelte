<script>
  import { Router, Route } from "svelte-routing";
  import Home from "./routes/Home.svelte";
  import Other from "./routes/Other.svelte";

  export let url = "";
</script>

<svelte:head>
  <!-- Main stuff goes in index.html, if it needs to be changed, do that here. -->
  <title>Page Title</title>
</svelte:head>

<Router {url}>
  <Route path="/" component={Home} />
  <Route path="/other" component={Other} />
</Router>
