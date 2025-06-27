<script lang="ts">
    import Container from "$lib/Container.svelte";
    import Navbar from "$lib/Navbar.svelte";
    import Course from "./CourseCard.svelte";
    import { base } from "$app/paths";
    import Footer from "$lib/Footer.svelte";

    class CourseInfo {
        name: string;
        cover: string;
        link: string;
        description: string;

        constructor(
            name: string,
            cover: string,
            link: string,
            description: string,
        ) {
            this.name = name;
            this.cover = base + cover;
            this.link = base + "/courses" + link;
            this.description = description;
        }
    }

    const courses = [
        new CourseInfo("C++ & DSA", "/cpp.jpg", "/cpp", "演算法競賽 & APCS"),
        new CourseInfo("Python", "/python.jpg", "/python", "簡單勝過複雜"),
        new CourseInfo("Unity", "/unity.jpg", "/unity", "利用 Unity 開發遊戲"),
        new CourseInfo("Web", "/web.jpg", "/web", "HTML/CSS/JavaScript"),
        new CourseInfo(
            "ML & AI",
            "/machine_learning.jpg",
            "/machine_learning",
            "機器學習 & 人工智慧",
        ),
        new CourseInfo(
            "Cyber Security",
            "/cyber_security.jpg",
            "/cyber_security",
            "基礎資安導論 & CTF",
        ),
    ];
</script>

<svelte:head>
    <title>課程 | 建北電資 29th</title>
</svelte:head>

<Navbar />
<Container>
    <ul class="courses">
        {#each courses as course}
            <li>
                <a href={course.link}>
                    <Course
                        name={course.name}
                        cover={course.cover}
                        description={course.description}
                    />
                </a>
            </li>
        {/each}
    </ul>
</Container>

<Footer />

<style>
    .courses {
        display: flex;
        margin: var(--spacing-8) 0;
        gap: var(--spacing-9);
        flex-wrap: wrap;
        justify-content: center;
    }

    li {
        list-style: none;
    }

    a {
        text-decoration: none;
    }
</style>
