<script lang="ts">
    import Section from "$lib/Section.svelte";
    import { base } from "$app/paths";
</script>

<div class="course-section">
    <Section title="課程" description="淺顯易懂、深入淺出" link="/29th-plus/courses" />
    <div class="cover">
        <img src="{base}/course.jpg" alt="cover" />
    </div>
</div>

<style>
    .course-section {
        margin-top: var(--spacing-7);
    }
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
