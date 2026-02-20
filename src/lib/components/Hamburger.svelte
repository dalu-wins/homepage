<script lang="ts">
    let { onclick }: { onclick: () => void; } = $props();
</script>

<button
    {onclick}
    type="button"
    class="group md:hidden glass-button flex flex-col justify-center items-center gap-1 w-10 h-10 rounded-2xl mr-6 z-15 outline-none"
    aria-label="Menu"
>
    {#each Array(3) as _, i}
        <span class="h-0.5 w-5 rounded-full transition-all duration-300
            bg-(--secondary-text) dark:bg-(--secondary-text-dark)
            group-hover:bg-(--primary-text) group-hover:dark:bg-(--primary-text-dark)">
        </span>
    {/each}
</button>