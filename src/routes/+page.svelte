<script lang="ts">
    import Profile from "$lib/components/profile.svelte";
    import Projects from "$lib/components/projects.svelte";
    import Navbar from "$lib/components/navbar.svelte";
    import Footer from "$lib/components/footer.svelte";
    import BackgroundTriangles from "$lib/components/BackgroundTriangles.svelte";
</script>

<div class="flex flex-col min-h-screen relative overflow-hidden p-4 container mx-auto px-8 grow gap-6">
    <Navbar />

    <main class="grow flex flex-col gap-6">
        <Profile />
        <Projects />
    </main>

    <BackgroundTriangles count={8} />

    <Footer />
</div>