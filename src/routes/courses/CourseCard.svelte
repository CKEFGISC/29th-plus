<script lang="ts">
    let { name, cover, description } = $props();
</script>

<div class="course_card">
    <div class="cover" style="background-image: url({cover});"></div>

    <div class="info">
        <h2 class="name">
            {name}
        </h2>

        <h3 class="description">
            {description}
        </h3>
    </div>
</div>

<style>
    .course_card {
        display: flex;
        width: 270px;
        flex-direction: column;
        background-color: hsl(0, 0%, 15%);
        border-radius: 10px;
        padding-bottom: 10px;
    }
    .course_card > .cover {
        height: 180px;
        width: 270px;
        border-radius: 10px;
        background-size: cover;
    }

    .name {
        color: white;
        font-size: 1.5rem;
        font-family: var(--font-1);
    }

    .description {
        font-family: var(--font-1);
        font-weight: 500;
        font-size: var(--text-base);
        color: lightgray;
    }

    .info {
        display: flex;
        flex-direction: column;
        margin: 1.5rem 1.5rem;
        gap: var(--spacing-2);
    }
</style>
