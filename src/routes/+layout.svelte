<script>
	import '../app.css';
	// import Navbar from './Navbar.svelte';
	import SideNav from './SideNav.svelte';
</script>

<!-- <Navbar /> -->

<div class="flex w-full h-full">
	<SideNav />
	<slot />
</div>

