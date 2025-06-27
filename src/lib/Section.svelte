<script lang="ts">
    export let title;
    export let description;
    export let link;
    
</script>

<section>
    <h2 class="title">{title}</h2>
    <h3 class="description">{description}</h3>
    <a href={link}>
        <button class="link-btn">瞭解更多</button>
    </a>
</section>

<style>
    section :global(*) {
        font-family: var(--font-1);
        color: var(--font-color);
    }

    section {
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: var(--spacing-4);
        margin: var(--spacing-8) 0;
    }

    .description {
        color: gray;
        font-weight: 400;
    }

    .link-btn {
        margin-top: 10px;
        border: none;
        border-radius: 5px;
        padding: var(--spacing-3);
        font-size: var(--text-xl);
        font-family: var(--font-1);
        background-color: oklch(0.76 0.1 264);
        color: black;
    }

    .link-btn:hover {
        cursor: pointer;
    }

    @media (max-width: 767px) {
        .title {
            font-size: var(--text-4xl);
        }

        .description {
            font-size: var(--text-xl);
        }

        .link-btn {
            font-size: var(--text-xl);
        }
    }

    @media (min-width: 768px) and (max-width: 991px) {
        .title {
            font-size: var(--text-5xl);
        }
        .description {
            font-size: var(--text-2xl);
        }
    }

    @media (min-width: 992px) {
        .title {
            font-size: var(--text-5xl);
        }
        .description {
            font-size: var(--text-2xl);
        }
    }
</style>
