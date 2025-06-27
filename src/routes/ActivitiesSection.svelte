<script lang="ts">
    import Section from "$lib/Section.svelte";
    import { base } from "$app/paths";
</script>


<div class="course-section">
    <Section title="活動" description="認識知心好友 & 各路電神" link="{base}/activities" />
    <div class="cover">
        <img src="{base}/activity.jpg" alt="cover" />
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
