<script lang="ts">
    import Container from "$lib/Container.svelte";
    import HeroSection from "./HeroSection.svelte";
    import CourseSection from "./CourseSection.svelte";
    import ActivitiesSection from "./ActivitiesSection.svelte";
    import Navbar from "$lib/Navbar.svelte";
    import { base } from "$app/paths";
    import Footer from "$lib/Footer.svelte";
</script>

<svelte:head>
    <title>首頁 | 建北電資 29th</title>
</svelte:head>

<Navbar />
<Container>
    <HeroSection />
    <div class="cover">
        <img src="{base}/cover.webp" alt="cover" />
    </div>

    <CourseSection />
    <ActivitiesSection />
</Container>

<Footer />

<style>
    .cover {
        display: flex;
        justify-content: center;
    }

    .cover > img {
        object-fit: contain;
        max-width: 100%;
        opacity: 0.8;
        border-radius: 1%;
    }
</style>
