<script lang="ts">
    import Navbar from "$lib/Navbar.svelte";
    import type { Slide } from "../CourseSlide.svelte";
    import Course from "../Course.svelte";

    const slides: Array<Slide> = [
        { name: "Python - 1 - 介紹 & 安裝、輸入 & 輸出、變數、List", link: "https://slides.com/d11231621/python-1" },
        { name: "Python - 2 - Tuple、Set、Queue & Stack、String、Dictionary", link: "https://slides.com/d11231621/python-2" },
        { name: "Python - 3 - if/else、for/while loop", link: "https://slides.com/d11231621/python-3" },
        { name: "Python - 4 - Function、Lambda、Class、Error Handling、Library", link: "https://slides.com/pomer0/python-4" },
        { name: "Discord Bot", link: "https://slides.com/lucasw/discord_bot" },
    ];
</script>

<svelte:head>
    <title>Python | 建北電資 29th</title>
</svelte:head>

<Navbar />
<Course name="Python" {slides}>
    <p>
        完全沒接觸過程式？想實際設計出實用的程式？覺得程式很難？別錯過 Python 小社！
    </p>
    <p>
        跟其他語言比起來，Python 簡單又強大。Python 的語法就跟英文沒兩樣（甚至更簡單！）， 而 Python 又支援不少第三方工具，所以能很輕鬆寫出功能強！大！的程式。
    </p>
    <p>
        沒寫過程式的話，來 Python 小社吧！
    </p>
</Course>
