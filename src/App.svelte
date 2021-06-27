<script>
	import Router from 'svelte-spa-router'
	import Navbar from './components/Navbar.svelte'
	import Sidebar from './components/Sidebar.svelte'
	import routes from './routes'
</script>

<Navbar/>

<main>
	<div class="columns is-fullheight">
		<div class="column is-2 is-mobile is-fullheight section">
			<Sidebar/>
		</div>
		<div class="column content">
			<Router {routes} />
		</div>
	</div>
</main>


<style>
	.content {
		padding-bottom: 0px;
	}
</style>