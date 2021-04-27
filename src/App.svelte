<script>
  import { Button, Modal, Dialog } from "attractions";
  import { Router, Route, Link } from "svelte-navigator";
  import Home from './Components/Home.svelte'
  import About from './Components/About.svelte'


</script>

<Router>
	<header>
	  <h1>History</h1>
  
	  <nav>
		<Link to="/">Home</Link>
		<Link to="about">About</Link>
		<Link to="profile">Profile</Link>
	  </nav>
	</header>
  
	<main>
	  <Route path="/">
		<Home />
	  </Route>
  
	  <Route path="/about">
		<About />
	  </Route>
	</main>
  </Router>
