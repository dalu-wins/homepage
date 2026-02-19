<script lang="ts">
    import Navbar from "$lib/components/navbar.svelte";
    import Footer from "$lib/components/footer.svelte";
    import Curriculum from "$lib/components/curriculum.svelte";
    import BackgroundTriangles from "$lib/components/BackgroundTriangles.svelte";
</script>

<div class="flex flex-col min-h-screen relative overflow-hidden">
    <Navbar />

    <main class="container mx-auto p-8 grow flex items-center relative z-10">
        <div class="grid lg:grid-cols-1 w-full items-center">
            <h1 class="text-4xl font-bold mb-10 dark:text-white mt-4">Curriculum</h1>
            <Curriculum />
        </div>
    </main>

    <BackgroundTriangles count={8} />

    <Footer />
</div>