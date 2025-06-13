<div class="container">
    <slot>
    </slot>
</div>

<style>
    @media (max-width: 767px) {
        .container {
            width: 90vw;
        }
    }

    @media (min-width: 768px) and (max-width: 991px) {
        .container {
            width: 80vw;
        }
    }

    @media (min-width: 992px) {
        .container {
            width: 60vw;
        }
    }

    .container {
        margin: 0 auto;
    }
</style>