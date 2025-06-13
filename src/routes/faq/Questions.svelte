<script lang="ts">
    import Question from "./Question.svelte";
</script>

<div class="questions">
    <Question question="沒有程式基礎也可以嗎？">
        <p>
            <strong>可以！</strong>
            多數課程設計面向初學者，即使上高中前沒接觸程式也沒關係。
        </p>
        <p>
            有幹部加入建北電資前完全沒碰過程式，在學長姐的教學下程式能力突飛猛進，甚至能自行開發大型專案或教其他人。
        </p>
        <p>
            學長姐都很有耐心，願意聽你們提出的每個問題，所以不懂的地方都可以問學長姐喔！
        </p>
    </Question>
    <Question question="有學長學弟制/學姐學妹制嗎？">
        <p>
            <strong>完全沒有!</strong>
            和某些特定社團比起來，建北電資可說是完全沒有長姐制。社團內的每個人都是平等相處的，沒有誰高誰低。
            也不會出現學長逼學弟留在學校補課、遇到學長姐一定要問好這些封建遺毒。
        </p>
        <p>
            學長跟學姐也都是很友善、講理的人，跟我們相處不用太拘束，就像一般朋友聊天就行！
        </p>
    </Question>
    <Question question="沒有電腦也可以嗎？">
        <strong>可以！</strong>
        <p>
            大社課跟放學小社課的上課地點都在電腦教室，可以使用建中或北一的電腦來上課。
        </p>
        <p>
            不過，最好還是自己帶電腦來上課喔！有一些課程需要安裝軟體，而這些軟體無法在建中或北一的電腦上跑。
            帶自己的電腦來也能省下每次安裝程式的時間。
        </p>
    </Question>
    <Question question="我想加入建電/北資，可是我正社沒上…">
        <p>
            沒關係，你還可以 <strong>地社</strong
            >喔！地社成員除了無法參與大社課之外，和<strong
                >正社成員沒有任何區別</strong
            >，一樣能<strong>來小社課跟參加活動</strong>。
        </p>
    </Question>
</div>

<style>
    .questions {
        display: flex;
        flex-direction: column;
        gap: 10px;
    }

    p {
        color: white;
    }
</style>
