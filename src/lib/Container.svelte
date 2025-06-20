<div class="container">
    <slot>
    </slot>
</div>

<style>
    @media (max-width: 767px) {
        .container {
            width: 100vw;
        }
    }
 
    @media (min-width: 768px) and (max-width: 991px) {
        .container {
            width: 80vw;
        }
    }

    @media (min-width: 992px) {
        .container {
            width: 65vw;
        }
    }

    .container {
        display: flex;
        flex-direction: column;
        align-items: center;
        margin: 0 auto;
    }
</style>
