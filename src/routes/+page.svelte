<script lang="ts">
    import Profile from "$lib/components/profile.svelte";
    import Projects from "$lib/components/projects.svelte";
    import Navbar from "$lib/components/navbar.svelte";
    import Footer from "$lib/components/footer.svelte";
    import BackgroundTriangles from "$lib/components/BackgroundTriangles.svelte";
</script>

<div class="flex flex-col min-h-screen relative overflow-hidden p-4 container mx-auto grow gap-4">
    <Navbar />

    <main class="grow flex flex-col gap-4">
        <Profile />
        <Projects />
    </main>

    <BackgroundTriangles count={8} />

    <Footer />
</div>