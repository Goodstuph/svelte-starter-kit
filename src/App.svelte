<script>
  import { Router, Route } from "svelte-routing";
  import Home from "./routes/Home.svelte";
  import Other from "./routes/Other.svelte";

  export let url = "";
</script>

<Router {url}>
  <Route path="/" component={Home} />
  <Route path="/other" component={Other} />
</Router>
