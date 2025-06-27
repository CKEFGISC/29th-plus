<div class="hero-section">
    <h1 class="title">
        <span class="program">程式</span>路上有你和我
    </h1>
    <blockquote>建北電資是個溫暖的大家庭</blockquote>
</div>

<style>
    @font-face {
        font-family: "ChenYuluoyan";
        /* src: url("/ChenYuluoyan-2.0-Thin.ttf") format("truetype"); */
        src: url("/test.ttf") format("truetype");
        font-weight: normal;
        font-style: normal;
    }

    .hero-section {
        font-family: "ChenYuluoyan", sans-serif;
        display: flex;
        flex-direction: column;
        align-items: center;
        padding: var(--spacing-6) 0;
        gap: var(--spacing-5);
    }

    .title {
        color: var(--font-color);
        font-size: var(--text-9xl);
        font-weight: 300;
        letter-spacing: -1.5px;
    }

    blockquote {
        color: var(--font-color);
        font-size: 2.5rem;
    }

    .program {
        color: hsl(48, 80%, 60%);
    }

    @media (min-width: 992px) {
        .hero-section {
            margin: var(--spacing-9) 0;
        }
    }

    @media (min-width: 768px) and (max-width: 991px) {
        .hero-section {
            margin: var(--spacing-8) 0;
        }
        .title {
            font-size: var(--text-8xl);
        }
    }

    @media (max-width: 767px) {
        .hero-section {
            margin: var(--spacing-7) 0;
        }
        .title {
            font-size: var(--text-7xl);
        }

        blockquote {
            font-size: var(--text-3xl);
        }
    }

    @media (max-width: 500px) {
        .hero-section {
            margin: var(--spacing-5) 0;
        }
        .title {
            font-size: var(--text-6xl);
        }

        blockquote {
            font-size: var(--text-3xl);
        }
    }

    @media (max-width: 360px) {
        .title {
            font-size: var(--text-5xl);
        }

        blockquote {
            font-size: var(--text-2xl);
        }
    }

</style>
