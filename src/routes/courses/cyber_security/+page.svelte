<script lang="ts">
    import Navbar from "$lib/Navbar.svelte";
    import type { Slide } from "../CourseSlide.svelte";
    import Course from "../Course.svelte";

    const slides: Array<Slide> = [
        { name: "Linux - 0 - 作業系統、Linux 介紹、常用指令", link: "https://slides.com/demonaarwu/linux-0" },
        { name: "Linux - 1 - VM、Python", link: "https://slides.com/demonaarwu/linux-1" },
        { name: "Git & GitHub 入門", link: "https://slides.com/demonaarwu/guide_to_git_and_github" },
        { name: "網路基礎概論", link: "https://slides.com/demonaarwu/networking-101" },
        { name: "CTF 介紹", link: "https://slides.com/ioker/capture_the_flag" },
        { name: "CTF - Crypto", link: "https://slides.com/ioker/ctf-cryto" },
        { name: "CTF - Forensic & Stego", link: "https://slides.com/ioker/ctf-forensic-n-stego" },
        { name: "CTF - Web", link: "https://slides.com/ioker/ctf-web" },
        { name: "CTF - Reverse", link: "https://slides.com/ioker/ctf-reverse" },
        { name: "CTF - End", link: "https://slides.com/ioker/ctf-end" },
    ];
</script>

<svelte:head>
    <title>資安 | 建北電資 29th</title>
</svelte:head>

<Navbar />

<Course name="資安" {slides}>
    <p>
        你對駭客的認知基本上都是錯的—駭客不會整天穿帽 T、輸入幾行 code 就能發射核彈、打字很快。
    </p> 
    <p>
        資安小社會讓你建立對駭客的專業領域—資訊安全的基本認識。講師從 Linux 講起，一路帶到網路、CTF 這些資安的基礎。
    </p>
    <p>
        這堂課不會讓你變成駭客，但絕對能讓你充分認識資安這個領域。
    </p>
</Course>
