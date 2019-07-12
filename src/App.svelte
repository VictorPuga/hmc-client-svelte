<script>
  import { Router, Link, Route } from "svelte-routing";
  import { Home, SignUp } from "./routes";
  import { Nav01 } from "./unicorn";
  export let url = "";
  const navButtons = [
    { title: "About", link: "/about" },
    { title: "Features", link: "/" },
    { title: "Contact us", link: "/" },
    { title: "Demo", link: "/" },
    { title: "Sign up", link: "/sign-up", outline: true }
  ];
</script>

<Router {url}>
  <div class="container">
    <Nav01 buttons={navButtons} icon="img/logos/self/square.png" />
  </div>
  <div class="container" style="margin-top: 60px">
    <Route path="sign-up" component={SignUp} />
    <Route path="/">
      <Home />
    </Route>
  </div>
</Router>
