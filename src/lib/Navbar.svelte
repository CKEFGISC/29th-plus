<script lang="ts">
    import { base } from "$app/paths";

    let open = false;

    function toggle_menu() {
        open = !open;
    }
</script>

<nav>
    <h2 class="club-name">
        <a href="{base}/">CKEFGISC 29th</a>
    </h2>

    <div class="hamburger-toggle" on:click={toggle_menu}>
        <span class="bar-1"></span>
        <span class="bar-2"></span>
        <span class="bar-3"></span>
    </div>

    <ul class:open={open} class="navlinks">
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

<style>

    .club-name,
    .club-name > a,
    .club-name > a:visited {
        color: white;
        font-family: "JetBrains Mono", sans-serif;
        font-weight: 500;
        /* border: 1px solid blue; */
        text-decoration: none;
    }

    nav {
        display: flex;
        width: 99vw;
        justify-content: space-between;
        align-items: center;
        padding: 0 15vw;
        margin-top: 10px;
        margin-bottom: 40px;
        height: 67px;
    }

    .navlinks {
        list-style: none;
        display: flex;
        justify-content: space-between;
        align-items: center;
        gap: 30px;
    }

    .navlink a {
        font-size: 18px;
        font-weight: 600;
        font-family: "Noto Sans TC";
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

    .hamburger-toggle span {
        height: 3px;
        width: 100%;
        border-radius: 10px;
        background-color: white;
    }

    .hamburger-toggle {
        width: 29px;
        height: 21px;
        top: 30px;
        right: 2rem;
        display: none;
        position: absolute;
        /*預設不顯示*/
        flex-direction: column;
        justify-content: space-between;
        align-items: flex-end;
        /*因為bar有長有短，所以靠左*/
    }

    @media (max-width: 767px) {
        .hamburger-toggle {
            display: flex;
        }

        .hamburger-toggle :hover {
            cursor: pointer;
        }
        nav {
            padding: 0 5vw;
        }

        .navlinks {
            display: none;
            flex-direction: column;
            position: absolute;
            z-index: 2;
            top: 67px;
            left: 0;
            width: 100%;
            background-color: black;
            text-align: center;
        }
        .navlinks li {
            padding: 20px;
        }

        .navlinks.open {
            display: block;
        }
    }

    @media (min-width: 768px) and (max-width: 991px) {
        nav {
            padding: 0 5vw;
        }
    }
</style>
