<script>
  import { Router, Link, Route } from "svelte-routing";
  import { Home, SignUp } from "./routes";
  import { Nav01 } from "./unicorn";
  export let url = "";
  const navButtons = [
    { title: "Nosotros", href: "#features" },
    { title: "Planes", href: "#subscription-plans" },
    { title: "FAQ", href: "#faq" },
    { title: "Entérate", href: "#newsletter-signup", outline: true }
  ];
</script>

<Router {url}>
  <div>
    <Nav01
      buttons={navButtons}
      icon="img/logos/self/square.png"
      title="Hacker Mafia Club" />
  </div>
  <div style="margin-top: 80px">
    <Route path="sign-up" component={SignUp} />
    <Route path="/" component={Home} />
  </div>
</Router>
