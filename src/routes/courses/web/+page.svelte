<script lang="ts">
    import type { Slide } from "../CourseSlide.svelte";
    import Course from "../Course.svelte";
    import Navbar from "$lib/Navbar.svelte";

    const slides: Array<Slide> = [
        { name: "網頁小社課 - 網頁基礎", link: "https://slides.com/laura07110717/copy-of" },
        { name: "網頁開發環境", link: "https://slides.com/laura07110717/minimal" },
        { name: "JavaScript", link: "https://slides.com/cloudream/javascript" },
        { name: "Backend[0]: Express", link: "https://slides.com/demonaarwu/backend-0"},
        { name: "Backend[1]: SQL", link: "https://slides.com/demonaarwu/backend-1-sql"},
    ];
</script>

<svelte:head>
    <title>網頁 | 建北電資 29th</title>
</svelte:head>

<Navbar />

<Course name="網頁" {slides}>
    <p>網頁無所不在—你現在滑的社網、平常滑的脆、Instagram、YouTube 背後都是網頁。所以，你該來這堂課學寫網頁！</p>
    <p>整堂課會從最基礎的網頁要素談起，結合每兩週的實作進行，一步步帶領學生做出完整、優美的網頁。</p>
    <p>每個網頁一定會有三個要素：HTML、CSS 和 JavaScript。HTML 是網頁的骨架、CSS 讓網頁有了血肉、JavaScript 讓網頁有了生命。 這門課的目標就是學好這三個要素，利用他們設計好的網頁。</p>
    <p>如果你想寫出像社網一樣棒的網站，或想寫個 Rickroll 網頁戳別人，網頁小社是你最好的選擇！</p>
</Course>
