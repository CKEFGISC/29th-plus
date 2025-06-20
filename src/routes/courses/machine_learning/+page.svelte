<script lang="ts">
    import type { Slide } from "../CourseSlide.svelte";
    import Course from "../Course.svelte";
    import Navbar from "$lib/Navbar.svelte";

    const slides: Array<Slide> = [
        { name: "機器學習社課第一堂 ", link: "https://slides.com/lucasw/ml-1"},
        { name: "機器學習社課第二堂 ", link: "https://slides.com/lucasw/ml-2"},
        { name: "機器學習社課第三堂 ", link: "https://slides.com/lucasw/ml-3"},
        { name: "機器學習社課第四堂 ", link: "https://slides.com/lucasw/ml-4"},
        { name: "機器學習社課第五堂 ", link: "https://slides.com/lucasw/ml-5"},
        { name: "機器學習社課第六堂 ", link: "https://slides.com/lucasw/ml-6"},
        { name: "機器學習社課第七堂 ", link: "https://slides.com/lucasw/ml-7"},
        { name: "機器學習社課第八堂", link: "https://slides.com/lucasw/ml-8"},
        { name: "機器學習社課第九堂", link: "https://slides.com/lucasw/ml-9"},
        { name: "機器學習社課第十堂", link: "https://slides.com/lucasw/ml-10"}
    ];
</script>

<svelte:head>
    <title>機器學習 | 建北電資 29th</title>
</svelte:head>

<Navbar />

<Course name="Unity 遊戲開發" {slides}>
    <p>
        喜歡遊戲嗎？想開發自己的遊戲？<s>你也玩原神嗎？</s>來遊戲設計小社吧！
    </p>
    <p>
        這堂課會從頭開始教 Unity，並使用 Unity 設計出屬於自己的遊戲！ Unity 是一個專門用來設計遊戲的<a href="https://zh.wikipedia.org/zh-tw/%E6%B8%B8%E6%88%8F%E5%BC%95%E6%93%8E">遊戲引擎</a>， 紀念碑谷、元氣騎士、Pokemon Go、<s>原神</s>這些知名遊戲都是利用 Unity 開發的。
    </p>
    <p>
        如果你想設計出夢想中的遊戲，那就來上課吧！
    </p>
</Course>
