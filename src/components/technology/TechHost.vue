<template>
   <section class="hosting-main">
        <div class="hosting-container container">
            <h2>Hosting Platforms</h2>
            <div class="host-logos">
                <div class="host-img">
                    <img src="../../assets/images/digitalocean.png" alt="img" />
                </div>
                <div class="host-img">
                    <img src="../../assets/images/amazoncloud.png" alt="img" />
                </div>
                <div class="host-img">
                    <img src="../../assets/images/googlecloud.png" alt="img" />
                </div>
                <div class="host-img">
                    <img src="../../assets/images/vurtle.png" alt="img" />
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: 'TechHost',
    }
</script>

<style scoped>
.hosting-main {
    padding: 2.5rem;
    border: 1px solid #cbd5e0;
}

.hosting-main .hosting-container {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.hosting-main .hosting-container h2 {
    letter-spacing: .1em;
    text-align: center;
    margin-bottom: 1.5rem;
    margin-top: 0px;
    font-size: 2.25rem;
    font-weight: 700;
    color: #2d3754;
    line-height: 1.8;
}

.hosting-main .hosting-container .host-logos {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    padding: 40px 20px;
}

.hosting-main .hosting-container .host-logos .host-img {
    width: 22%;
}

.hosting-main .hosting-container .host-logos .host-img img {
    width: 100%;
}

@media (max-width: 479px) and (min-width: 320px) {
 .hosting-main .hosting-container .host-logos{
       flex-wrap: wrap;
   }
   .hosting-main .hosting-container .host-logos .host-img {
    width: 100%;
}
}

@media (max-width: 684px) and (min-width: 575px) {}

@media (max-width: 767px) and (min-width: 685px) {}

@media (max-width: 991px) and (min-width: 768px) {}

@media (max-width: 574px) and (min-width: 480px) {}

@media (max-width: 1199px) and (min-width: 1024px) {}
</style>