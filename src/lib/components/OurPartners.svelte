<script>
        import Carousel from 'svelte-carousel';
    import { browser } from '$app/environment';

    var carousel;

    
</script>

<div class="mx-32">
    <p class="text-gray-500 text-center font-semibold">Tensax Innovation Lab is trusted by various organisations throughout the world</p>
    {#if browser}
    <Carousel
        bind:this={carousel}
        particlesToShow={4}
        autoplayDuration={0}

    duration={2000}
    autoplay
    timingFunction="linear"
    dots={false}
    arrows={false}
    swiping={false}
    >
        {#each Array(8) as _, i}
            <img class="w-4 h-40" src="tensax/company{i+1}.png" alt="">
        {/each}
    </Carousel>
    {/if}
</div>