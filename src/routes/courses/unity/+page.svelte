<script lang="ts">
    import type { Slide } from "../CourseSlide.svelte";
    import Course from "../Course.svelte";
    import Navbar from "$lib/Navbar.svelte";

    const slides: Array<Slide> = [
        { name: "Unity 第一堂", link: "https://slides.com/d11230618/ckefgisc_unity_class1" },
        { name: "Unity 第二堂", link: "https://slides.com/aprilfirst/code" },
        { name: "Unity 第 3.5 堂", link: "https://slides.com/d11230618/ckefgisc_unity_class3" },
        { name: "Unity 第 N 堂 - Tilemap", link: "https://slides.com/jellyyfish/unity-tilemap" },
        { name: "Unity - Prefab", link: "https://slides.com/aprilfirst/code-ef6086" },
        { name: "Unity 第 N+1 堂 - UI", link: "https://slides.com/jellyyfish/unity-ui" },
        { name: "Unity 第四、五堂", link: "https://slides.com/d11230618/unity_class4" },
        { name: "Unity 第 N+2 堂", link: "https://slides.com/jellyyfish/unity-project" },
        { name: "Unity 部署", link: "https://slides.com/bethchen/unity_n"}
    ];
</script>

<svelte:head>
    <title>Unity 遊戲開發 | 建北電資 29th</title>
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
