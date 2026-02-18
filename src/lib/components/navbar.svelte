<script>
    import { Navbar, NavBrand, NavHamburger, NavUl, NavLi, DarkMode } from "flowbite-svelte";

</script>

<Navbar class="p-6 text-(--navbar) dark:text-(--navbar-dark) bg-(--bg-navbar) dark:bg-(--bg-navbar-dark)">
    <NavBrand href="/">
        <span
            class="self-center text-xl font-semibold whitespace-nowrap"
            >homepage</span
        >
    </NavBrand>
    <div class="flex items-center gap-2 md:order-2">
        <NavHamburger />
        <NavUl class="md:flex-row md:gap-6 px-2">
            <NavLi href="#profile">Profile</NavLi>
            <NavLi href="#projects">Projects</NavLi>
            <NavLi href="#curriculum">Curriculum</NavLi>
        </NavUl>
        <DarkMode />
    </div>
</Navbar>