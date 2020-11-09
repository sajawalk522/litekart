<template>

    <div class="cards">
        <div class="card-logo">
            <img :src="require(`../../assets/images/${boxes.image}`)" alt="img" />
        </div>
        <div class="card-text">
            <h3>{{boxes.heading}}</h3>
            <p>{{boxes.text}}</p>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'CardBox',
        props: {
            boxes: [],
        }
    }
</script>

<style scoped>
 .cards {
    width: 100%;
    text-align: left;
    display: flex;
    justify-content: center;
    align-items: center;
    
}

 .cards .card-logo {
    margin-right: 2rem;
}

 .cards .card-logo img {
    width: 48px;
    height: 48px;
}

 .cards .card-text h3 {
    letter-spacing: .05em;
    margin-bottom: .5rem;
    margin-top: 0;
    color: #2d3754;
    line-height: 1.8;
    font-weight: 400;
    font-size: 1.25rem;
}

 .cards .card-text p {
    text-align: left;
    color: #1a202c;
    letter-spacing: .05em;
    color: #2d3754;
    line-height: 1.5;
    font-weight: 400;
    font-size: 1rem;
}
@media (max-width: 479px) and (min-width: 320px) {
  .cards{
       width: 100%;
       flex-direction: column;
       text-align: center;
   }
   .cards .card-text p{
       text-align: center;
   }
}

@media (max-width: 684px) and (min-width: 575px) {}

@media (max-width: 767px) and (min-width: 685px) {}

@media (max-width: 991px) and (min-width: 768px) {}

@media (max-width: 574px) and (min-width: 480px) {}

@media (max-width: 1199px) and (min-width: 1024px) {}
</style>