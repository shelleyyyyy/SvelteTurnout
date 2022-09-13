<script>
    import Info from "./Info.svelte";
    import InfoHeader from "./InfoHeader.svelte";
    
    export let title;
    export let description;
    export let author;
    export let date;
    export let info;
</script>

<section>
    <div class="p-6 bg-white shadow-sm rounded-lg hover:shadow-lg cursor-pointer duration-300 m-5">
        <h1 class="text-5xl font-bold text-left pb-2">{title}</h1>
        <p class="content">{description}</p>
        <div class="p-2 flex flex-wrap justify-center">
            <!-- <InfoHeader></InfoHeader> -->
            {#each info as item}
                <Info title={item.title} value={item.value} />
            {/each}
        </div>
    </div>
</section>

<style>

</style>