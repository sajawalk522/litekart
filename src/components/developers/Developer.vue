<template>
    <div>
         <ForDevelopers />
         <section class="included-main big-cards" >
        <div class="icluded-container" >
            <div class="includ-head">
                <h2>WHAT’S INCLUDED</h2>
                <p>Get 100+ premium features out of the box with litekart's integrated onetime pricing</p>
            </div>
            <div class="includ-cards">
                <div v-for="(card, index) in cards" :key="index">
                    <CardBox :boxes="card"/>
                </div>
            </div>
        </div>
    </section>
    </div>
</template>

<script>
import ForDevelopers from './ForDeveloper';
import CardBox from '../include-card/CardBox';
    export default {
        name: 'Developer',
         props: {
          set: String,
          DevCard: [],
        },
        components: {
            ForDevelopers,
            CardBox
        },
        data: function () {
            return {
               
               cards: [
                  
                   {   
                       image: 'building-solid.svg',
                       heading: 'Build a beautiful and fast ecommerce website',
                       text: 'We create a fully customized, responsive online store that speaks to your customers and showcases your products with all essential feaures. Choose from high-converting online store designs optimized for fast page-load across devices and designed especially for major ecommerce industries. Our design includes Cloud Based Image Optimizer to automatically optimize each image for browser and device.',
                   },
                   {
                       image: 'wrench-solid.svg',
                       heading: 'Completely customize your website',
                       text: 'Our highly customizable platform lets you create the unique ecommerce store for you with perfect shopping experience quickly. Work with a developer to customize any aspect of your website’s design and shopping cart.',
                   },
                   {
                       image: 'comment-dots-solid.svg',
                       heading: 'Deliver a personalized experience',
                       text: 'Personalize your site to better engage and convert shoppers using a flexible modular code base, conditional logic and access to language files.',
                   },
                   {
                       image: 'mobile-alt-solid.svg',
                       heading: 'The best solution for selling on mobile',
                       text: 'A 1-second delay in page load can decrease conversion by 7%. Online stores from Litekart are blazing fast on cloud infrastructure, with an average page load time under 2 seconds – resulting in faster page browsing times, improved conversion, and better customer experience.',
                   },

                   {
                       image: 'file-signature-solid.svg',
                       heading: 'Faster sites, higher conversion',
                       text: 'Personalize your site to better engage and convert shoppers using a flexible modular code base, conditional logic and access to language files.',
                   },
                   {
                       image: 'medal-solid.svg',
                       heading: 'Sitewide HTTPS boosts conversion and search rankings',
                       text: 'All Litekart plans offer HTTPS across your entire site. That builds confidence amoung shoppers while they know your online store is secure from the first page they visit through checkout, and ensures you’re complying with Google’s latest guidelines to maximize SEO.',
                   },
                   {
                       image: 'search-solid (1).svg',
                       heading: 'Rank higher with best-in-class SEO',
                       text: 'Our sites are built for better search engine rankings using search-friendly html, sitewide HTTPS, optimized URLs, automatic sitemaps, optimized images, microdata and more. We also give you full control to customize your URLs, titles, header tags and metadata.',
                   },
                   {
                       image: 'share-alt-solid.svg',
                       heading: 'Social',
                       text: 'Features for social media promotion is pre integrated. facebook, twitter, instgram sharing will auto detect image and content',
                   },
                   {
                       image: 'tape-solid.svg',
                       heading: 'Build your own integrations with our powerful API',
                       text: 'Our flexible, open API lets you build custom integrations with whatever software you count on to run your business. Connect with all the most important parts of our platform, including Products, Customers, Orders, Payments, Shipping and more.',
                   },
                   {
                       image: 'arrow-down-solid.svg',
                       heading: 'Recover 20% of abandoned carts',
                       text: 'Up to 60% of online shopping carts are abandoned before checkout. Recover those lost sales with our abandoned cart saver and optimize for the traffic you already receive. This conversion tool automatically sends shoppers a customizable series of emails that motivates them to complete a purchase.',
                   },
                   {
                       image: 'chart-bar-solid.svg',
                       heading: 'Improve conversion rates by 22% with a streamlined checkout',
                       text: 'Our single-page checkout improves conversion up to 22% by making it faster and easier to complete a purchase. We’ve built in conversion-boosting features like mobile optimization, account creation for faster checkouts, guest checkout, and dedicated SSL support that enables shoppers to stay on your domain during checkout.',
                   },
                   {
                       image: 'file-code-solid.svg',
                       heading: 'A developers dream',
                       text: 'Quickly develop elegant solutions to complex problems using our open APIs. Our RESTful architecture allows you to code in the language of your choice. Unthrottled API calls support hundreds of requests per second without bottlenecks, letting you parallelize work and improve efficiency. All APIs are documented using the Postman.',
                   },
                    {
                       image: 'funnel-dollar-solid.svg',
                       heading: 'Improve search effectiveness with filtering',
                       text: 'Faceted search helps shoppers quickly find the products they want using filters like size, color, brand and even custom attributes. Adding filters with faceted search can increase conversion by as much as 30%',
                   },
                   {
                       image: 'user-tag-solid.svg',
                       heading: 'Incentivize buyers with built-in coupons and discounting',
                       text: 'Win new customers and reward repeat buyers using our flexible discounting tools. From a single location in your control panel, you can set up cart based discount or product based percentage discounts, dollar-off discounts, shipping discounts, or promotions like buy one, get one free.',
                   },
                   {
                       image: 'star-solid.svg',
                       heading: 'Boost shopper confidence with product reviews',
                       text: 'Featuring product reviews increases sales by 17% on average. They’re built right into Litekart at no extra cost, and you can automatically email buyers a few days after purchase to ask for a review.',
                   },
                   {
                       image: 'star-solid.svg',
                       heading: 'Get world-class support',
                       text: 'Get expert help 24/7, with premium services available for Enterprise merchants. Talk directly to our lead developer and discuss about bug fixes or new feature requirements.',
                   },
                   {
                       image: 'hands-helping-solid.svg',
                       heading: 'Migration and onboarding help',
                       text: 'Switching platforms or launching a new store can feel overwhelming, but we dramatically simplify the process. You have access to our onboarding dedicated personal consultant.',
                   },
               ]
            }
        }
    }
</script>


<style scoped>
.included-main {
    padding: 0.5rem;
    background-color: #f7fafc;
    margin-top: 30px;
    display: flex;
    justify-content: center;
}
.included-main .icluded-container {
    width: 880px;
}
.included-main .icluded-container .includ-head h2 {
    letter-spacing: .05em;
    color: #2d3754;
    line-height: 1.8;
    font-weight: 700;
    font-size: 2.25rem;
    margin-top: 0;
    margin-bottom: .5rem;
    text-align: center;
}

.included-main .icluded-container .includ-head p {
    letter-spacing: .1em;
    text-align: center;
    color: #1a202c;
    margin-bottom: 2rem;
    font-size: 1.25rem;
    line-height: 1.8;
    font-weight: 400;
}

.included-main .icluded-container .includ-cards {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    align-items: flex-start;
}
.included-main .icluded-container .includ-cards>div{
    width: 40%;
    margin: 15px;
    padding: 2rem 1.5rem;
    border-radius: .5rem;
    background-color: #fff;
    box-shadow: 0 4px 6px -1px rgba(0, 0, 0, .1), 0 2px 4px -1px rgba(0, 0, 0, .06);
    border: 1px solid #e2e8f0;
}

.big-cards{
    background-color:unset;

}
.big-cards .icluded-container {
    width: 100%;
}
</style>