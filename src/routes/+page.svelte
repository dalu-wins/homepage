 <script lang="ts">
    import { Navbar, NavBrand, NavLi, NavUl, NavHamburger, DarkMode } from "flowbite-svelte";
</script>

<Navbar>

    <NavBrand href="/">
        <span class="self-center text-xl font-semibold whitespace-nowrap dark:text-white">Daniil Wins</span>
    </NavBrand>

    <div class="flex items-center gap-2 md:order-2">
        <NavHamburger />

        <NavUl class="md:flex-row md:gap-6 px-2">
            <NavLi href="/">Profile</NavLi>
            <NavLi href="/projects">Projects</NavLi>
            <NavLi href="/curriculum">Curriculum</NavLi>
            <NavLi href="/contact">Contact</NavLi>
        </NavUl>

        <DarkMode />
    </div>

</Navbar>

