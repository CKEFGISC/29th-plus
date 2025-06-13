<script lang="ts">
    let { question } = $props();
</script>

<details class="qa">
    <summary class="question">
        <h2>
            Q: {question}
        </h2>
    </summary>
    <div class="answer">
        <slot>

        </slot>
    </div>
</details>

<style>
    summary {
        list-style: none;
        margin-bottom: 15px;
    }
    details {
        font-size: 1.3rem;
    }
    .question > h2 {
        display: inline;
        font-weight: 400;
        color: white;
    }
</style>