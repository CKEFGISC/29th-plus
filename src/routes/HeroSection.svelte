<div class="hero-section">
    <h1 class="title">
        <span class="program">程式</span>
        路上有你和我
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
        font-family: "ChenYuluoyan";
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 30px;
        margin: 50px 0;
    }

    .title {
        color: white;
        font-size: 5rem;
        font-weight: 300;
    }

    blockquote {
        color: white;
        font-size: 2.5rem;
    }

    .program {
        color: #e9ce56;
    }

    @media (max-width: 767px) {
        .title {
            font-size: 4rem;
        }

        blockquote {
            font-size: 2rem;
        }
    }

    @media (max-width: 375px) {
        .title {
            font-size: 3rem;
        }
    }

</style>