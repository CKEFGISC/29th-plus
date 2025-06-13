<script lang="ts">
    import { base } from "$app/paths";
</script>

<header>
    <nav>
        <h2 class="club-name">
            <a href="{base}/">CKEFGISC 29th</a>
        </h2>

        <ul class="navlinks">
            <li class="navlink">
                <a href="{base}/courses">課程</a>
            </li>
            <li class="navlink">
                <a href="{base}/activities">活動</a>
            </li>
            <li class="navlink">
                <a href="{base}/faq">FAQ</a>
            </li>
            <li class="navlink">
                <a href="{base}/about">關於</a>
            </li>
        </ul>
    </nav>
</header>

<style>
    @import url("https://fonts.googleapis.com/css2?family=JetBrains+Mono:ital,wght@0,100..800;1,100..800&display=swap");

    .club-name,
    .club-name > a,
    .club-name > a:visited {
        color: white;
        font-family: "JetBrains Mono", sans-serif;
        font-size: xx-large;
        font-weight: 500;
        /* border: 1px solid blue; */
        text-decoration: none;
    }

    header {
        display: flex;
        justify-content: center;
        width: 100vw;
        padding: 20px 0;
        /* border: 1px solid black; */
    }

    nav {
        display: flex;
        justify-content: space-between;
    }

    .navlinks {
        display: flex;
        justify-content: space-between;
        align-items: center;
        list-style: none;
        /* border: 1px solid red; */
        width: 20vw;
    }

    .navlink {
        font-family: "Noto Sans TC";
        font-size: 1.5rem;
    }

    .navlink > a,
    .navlink > a:visited {
        color: white;
        text-decoration: none;
        font-weight: 400;
    }

    .navlink > a:hover {
        color: rgb(241, 211, 110);
    }

    @media (max-width: 767px) {
        nav {
            width: 90vw;
        }
    }

    @media (min-width: 768px) and (max-width: 991px) {
        nav {
            width: 80vw;
        }
    }

    @media (min-width: 992px) {
        nav {
            width: 70vw;
        }
    }
</style>
