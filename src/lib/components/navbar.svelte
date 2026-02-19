<script>
	import { Navbar, NavBrand, NavHamburger, DarkMode } from 'flowbite-svelte';
    import NavLinks from './navLinks.svelte';

	let menuOpen = $state(false);
	const toggleMenu = () => (menuOpen = !menuOpen);
</script>

<Navbar
	class="w-full z-20 glass drop-shadow-md rounded-4xl"
>
	<NavBrand href="/">
		<span class="self-center text-xl font-semibold whitespace-nowrap m-4 text-(--navbar) dark:text-(--navbar-dark)">
			homepage
		</span>
	</NavBrand>

	<div class="flex items-center gap-2 md:order-2">
		<DarkMode
			class="hover:bg-(--bg-nav-hover) dark:hover:bg-(--bg-nav-hover-dark) hover:text-black dark:hover:text-white text-(--secondary-text) dark:text-(--secondary-text-dark) mr-0 md:mr-6"
		/>
		<NavHamburger onclick={toggleMenu} class="md:hidden mr-6" />
	</div>

	<NavLinks {menuOpen} />
</Navbar>