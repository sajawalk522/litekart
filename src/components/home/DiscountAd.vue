<template>
     <section class="discount-container">
        <div class="discount-text">
            <p>Up to <span>90% discount</span> for qualified startups.</p>
        </div>
            <a href="#" class="btn btn-yellow">LET'S TALK </a>
    </section>
</template>

<script>
    export default {
        name: 'DiscountAd'
    }
</script>

<style scoped>
.discount-container {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 1.5rem 0;
    background-color: #44337a;
}

.discount-text p {
    font-size: 1.5rem;
    --text-opacity: 1;
    color: #fff;
}

.discount-text p span {
    color: #00bb6e;
    font-weight: 700;
}
.btn-yellow {
    background-color: #fdc700;
    color: #000!important;
    font-weight: 500!important;
}
@media (max-width: 479px) and (min-width: 320px) {
    .discount-container {
        flex-wrap: wrap;
        text-align: center;
    }
    .arich-card {
        flex-wrap: wrap;
    }
    .arich-card .card-dev {
        width: 100%;
    }
}

@media (max-width: 684px) and (min-width: 575px) {}

@media (max-width: 767px) and (min-width: 685px) {}

@media (max-width: 991px) and (min-width: 768px) {}

@media (max-width: 574px) and (min-width: 480px) {}

@media (max-width: 1199px) and (min-width: 1024px) {}
</style>