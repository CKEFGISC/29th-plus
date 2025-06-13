<script lang="ts">
    import Container from "$lib/Container.svelte";
    import HeroSection from "./HeroSection.svelte";
    import Navbar from "$lib/Navbar.svelte";
    import Cover from "$lib/assets/cover.webp";
</script>

<Navbar />
<Container>
    <HeroSection />
    <div class="cover">
        <img src={Cover} alt="cover" />
    </div>
</Container>

<style>
    .cover > img {
        display: block;
        object-fit: contain;
        max-width: 95%;
        border-radius: 2.5%;
        opacity: 0.7;
    }

    .cover {
        display: flex;
        justify-content: center;
    }
</style>
