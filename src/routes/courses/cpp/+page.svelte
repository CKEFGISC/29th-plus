<script lang="ts">
    import Navbar from "$lib/Navbar.svelte";
    import type { Slide } from "../CourseSlide.svelte";
    import Course from "../Course.svelte";

    const slides: Array<Slide> = [
        { name: "C++ 基礎語法", link: "https://slides.com/keaucucal/c" },
        { name: "C++ 基礎語法第二堂", link: "https://slides.com/wenian/cpp-1/" },
        { name: "C++ STL 之一", link: "https://slides.com/oct0920/template/" },
        { name: "C++ STL 之二", link: "https://slides.com/oct0920/copy-of-template-209f73" },
        { name: "基礎演算法之一 - 枚舉、剪枝、Greedy", link: "https://slides.com/keaucucal/algo-0" },
        { name: "基礎演算法之二 - 雙指針、二分搜、分治", link: "https://slides.com/keaucucal/algo-1" },
        { name: "基礎圖論之一", link: "https://slides.com/wenian/graph-theory0" },
        { name: "Dynamic Programming - 1", link: "https://slides.com/keaucucal/dp" },
        { name: "Dynamic Programming - 2", link: "https://slides.com/wenian/dynamic-programming-ii" },
        { name: "基礎圖論之二", link: "https://slides.com/keaucucal/graph-1" },
        { name: "數論之一", link: "https://slides.com/keaucucal/math" },
        { name: "數論之二", link: "https://slides.com/wenian/math-1" },
        { name: "進階資料結構", link: "https://hackmd.io/@keaucucal/range_queries"},
        { name: "More Segment Tree", link: "https://slides.com/wenian/segment-trees"}
    ];
</script>

<svelte:head>
    <title>C++ & 演算法 | 建北電資 29th</title>
</svelte:head>

<Navbar />

<Course name="C++ & 演算法" {slides}>
    <p>想考 APCS 嗎？想歐趴高中資訊課嗎？想鍛鍊解決程式問題的能力嗎？來演算法小社準沒錯！</p>
    <p>這堂課從最基礎的 C++ 教起，接著帶到演算法競賽（競程）常用的資料結構和演算法，逐漸帶領學生學會解決競程難題。</p>
    <p>
        上完這堂課後，高中資訊課、APCS、<s>TOI</s> 根本 piece of 小蛋糕！
    </p>
</Course>
