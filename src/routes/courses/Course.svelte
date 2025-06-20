<script lang="ts">
    import ArticleContainer from "$lib/ArticleContainer.svelte";
    import CourseSlides from "./CourseSlides.svelte";
    import type { Slide } from "./CourseSlide.svelte";
    import Footer from "$lib/Footer.svelte";

    let { name, slides }: { name: string; slides: Array<Slide> } = $props();
</script>

<div class="course">
    <ArticleContainer>
        <h1 class="name">{name}</h1>
        <h3>介紹</h3>
        <slot />
        <h3>簡報</h3>
        <CourseSlides {slides} />
    </ArticleContainer>
</div>

<Footer />
