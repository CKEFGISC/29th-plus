<script lang="ts">
    const year = new Date().getFullYear();
</script>

<footer>
    <p>Copyright © {year} CKEFGISC 建北電資 29th </p>
</footer>

<style>
    * {
        font-family: var(--font-1);
    }
    p {
        text-align: center;
        font-size: var(--text-base);
        color: darkgray;
    }
    footer {
        display: flex;
        flex-direction: column;
        justify-content: center;
        width: 100vw;
        margin: var(--spacing-6) auto;
    }

    @media (max-width: 767px) {
        p {
            font-size: var(--text-sm);
        }
    }
</style>
