<svelte:head>
	<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta1/dist/css/bootstrap.min.css"/>
	<link rel="stylesheet" href="https://db.onlinewebfonts.com/c/729005f056820f234a1315de6d2ce8fb?family=Arquitecta"/>
	<link rel="stylesheet" href="https://db.onlinewebfonts.com/c/bf9f5d50c1b928ff21436517a1a95ad9?family=Proxima+Nova"/>
</svelte:head>

<script>
	import { Router, Link, Route } from "svelte-routing";

	import Home from "./pages/Home.svelte";
	import Login from "./pages/Login.svelte";
	import Instructors from "./pages/Instructors.svelte";
	import Explores from "./pages/Explores.svelte";

	export let url = "";
</script>

<Router url="{url}">
	<Route path="/login"><Login /></Route>
	<Route path="/instructors"><Instructors /></Route>
	<Route path="/explores"><Explores /></Route>
	<Route path="/"><Home /></Route>
</Router>