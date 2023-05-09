<script>
    import { userDefaultImages } from "$lib/gameAssets";
    export let src = '';
    export let width = "60px";
    export let height = "60px";
</script>

{#if src != ''}
    <img src={src} alt="custom profile" width={width} height={height}>
{:else}
    <img src={userDefaultImages.profile} alt="default profile" width={width} height={height}>
{/if}

<style>
    img {
        border-radius: 50%;
        object-fit: cover;
    }
</style>



