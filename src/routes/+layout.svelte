<script lang="ts">
    import {profile} from "$lib/display/profile";
    import "../app.css";
    let { children } = $props();
</script>

<svelte:head>
    <title>homepage</title>
    <link rel="icon" href={profile.avatarUrl} />
    <meta 
        name="description" 
        content="Explore the portfolio of dalu-wins. Featuring mobile and web development projects, a curriculum and contact information." 
    />
</svelte:head>

{@render children()} 