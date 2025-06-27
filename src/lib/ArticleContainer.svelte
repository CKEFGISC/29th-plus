<div class="container">
    <slot></slot>
</div>

<style>
    .container :global(h1),
    .container :global(h2),
    .container :global(h3),
    .container :global(p),
    .container :global(a) {
        font-family: var(--font-1);
    }

    .container :global(h1) {
        font-size: var(--text-5xl);
    }

    .container :global(h3) {
        font-size: var(--text-3xl);
    }

    .container :global(p) {
        font-size: var(--text-xl);
    }

    .container :global(a),
    .container :global(a:visited) {
        color: hsl(197 100% 70.8%);
        font-size: var(--text-xl);
    }

    @media (max-width: 767px) {
        .container {
            width: 90vw;
        }

        .container :global(h1) {
            font-size: var(--text-4xl);
        }

        .container :global(h3) {
            font-size: var(--text-2xl);
        }

        .container :global(p) {
            font-size: var(--text-lg);
        }

        .container :global(a),
        .container :global(a:visited) {
            color: hsl(197 100% 70.8%);
            font-size: var(--text-lg);
        }
    }

    @media (min-width: 768px) and (max-width: 991px) {
        .container {
            width: 80vw;
        }
    }

    @media (min-width: 992px) {
        .container {
            width: 60vw;
        }
    }

    .container {
        margin: 0 auto;
        margin-top: var(--spacing-8);
    }

    .container :global(h1) {
        margin-top: 30px;
        margin-bottom: 30px;
    }

    .container :global(h3) {
        margin-top: var(--spacing-4);
        margin-bottom: var(--spacing-4);
    }

    .container :global(p) {
        margin-top: var(--spacing-3);
        margin-bottom: var(--spacing-3);
    }
</style>
