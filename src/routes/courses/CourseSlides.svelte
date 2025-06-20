<script lang="ts">
    import CourseSlide from "./CourseSlide.svelte";
    import type { Slide } from "./CourseSlide.svelte";

    let { slides }: { slides: Array<Slide> } = $props();

</script>

<ul class="course-slides">
    {#each slides as slide}
        <li class="slide">
            <CourseSlide course_slide={slide} />
        </li>
    {/each}
</ul>

<style>
    .slide {
        list-style: none;
    }
</style>
