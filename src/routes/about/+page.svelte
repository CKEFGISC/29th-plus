<script lang="ts">
    import Footer from "$lib/Footer.svelte";
    import Navbar from "$lib/Navbar.svelte";
    import { base } from "$app/paths";
</script>

<svelte:head>
    <title>關於 | 建北電資 29th</title>
</svelte:head>

<Navbar />
<div class="container">
    <div class="blocks">
        <div class="about-ckefgisc block">
            <img src="{base}/ckefgisc.webp" alt="CKEISC 44th" class="ckeisc-logo" />
            <div class="info">
                <h1>建北電資</h1>
                <p>建北電資為建中電研和北一資研兩社組成的大社團，至今已是橫跨三十年的大家庭。</p>
                <p>兩社平時會在放學舉辦小社課，並會在假日舉辦大型活動（四大獵祭）。</p>
            </div>
        </div>
        <div class="about-ckeisc block">
            <img src="{base}/ckeisc_44th.jpg" alt="" />
            <div class="info">
                <h1>建中電研</h1>
                <p>建中電研為建中首屈一指的學術性社團，由一群程式愛好者組成。</p>
                <p>大社課由幹部教授各種程式知識。放課則和北資一起舉辦，主題橫跨演算法、遊戲開發、人工智慧、網頁等。</p>
            </div>
        </div>
        <div class="about-fgisc block">
            <img src="{base}/fgisc_38th.jpg" alt="" />
            <div class="info">
                <h1>北一資研</h1>
                <p>北一資研是以程式為主題的學術性社團。 </p>
                <p>大社課由專業社師教授 C++ ，平時中午小社課和放學與建電的聯課則有諸多不同領域。偶爾會舉辦活動聯繫感情。</p>
            </div>
        </div>
    </div>
</div>
<Footer />

<style>
    * {
        font-family: var(--font-1);
    }
    
    .container {
        display: flex;
        justify-content: center;
        margin: 0 auto;
    }

    .info > h1 {
        font-size: var(--text-3xl);
        font-weight: 600;
    }

    .info > p {
        font-size: var(--text-xl);
    }

    img {
        height: 200px;
        width: 200px;
    }

    @media (min-width: 992px) {
        .container {
            width: 65vw;
        }
        .info {
            height: 200px;
            padding-left: var(--spacing-5);
            max-width: 800px;
        }
    }

    @media (min-width: 768px) and (max-width: 991px) {
        .container {
            width: 85vw;
        }
        .info {
            height: 200px;
            padding-left: var(--spacing-5);
        }
    }

    @media (max-width: 767px) {
        .blocks {
            width: 300px;
        }

        .block {
            flex-direction: column;
            gap: var(--spacing-5);
            align-items: center;
        }

        img {
            width: 300px;
            height: auto;
            border: 1px solid #333331;
            border-radius: 10%;
        }

        @media (max-width: 360px) {
            .info > h1 {
                font-size: var(--text-2xl);
            }

            .info > p {
                font-size: var(--text-lg);
            }
        }
    }

    .blocks {
        display: flex;
        flex-direction: column;
        justify-content: center;
        gap: var(--spacing-8);
        margin-top: var(--spacing-8);
    }

    .block {
        display: flex;
        align-items: center;
    }

    .info {
        display: flex;
        flex-direction: column;
        gap: var(--spacing-4);
        flex-grow: 1;
    }

</style>
