<template>
<div>
   <!-- section header end -->
    <section class="header-section">
      <div class="since-primary">
        <div class="container">
          <h6>800+ custom stores implementated since 2014</h6>
        </div>
      </div>
      <div class="header-primary">
        <div class="header container">
          <div class="primary-list active-class">
            <div class="logo active-logo">
                <router-link to="/">
                <div><img src="../../assets/images/logo.svg" /></div>
                <div class="logo-text"><span>Litekart</span></div>
              </router-link>
            </div>
            <div class="navigation-list">
              <ul>
                <li class="hover-dropdown"><router-link to="features">FEATURES</router-link>
                  <!-- dorpdown -->
                  <DropDown />
                </li>
                <li><router-link to="/live-projects">LIVE PROJECTS</router-link></li>
                <li><router-link to="/litekart-story">STORY</router-link></li>
                <li><router-link to="/technology">TECHNOLOGY</router-link></li>
                <li><router-link to="/ecommerce-developer">DEVELOPERS</router-link></li>
              </ul>
            </div>
          </div>
          <div class="lets-talk">
            <div>
                <div class="navigation-list price-list active-class">
              <ul>
                <li><router-link to="/pricing">PRICING</router-link></li>
              </ul>
            </div>
            </div>
            <div>
                <router-link to="/contact" class="btn btn-talk">Let's talk</router-link>
            </div>
          </div>
        </div>
      </div>
    
    </section>
    <!-- section header end -->
<!-- Mobile header start  -->
    <div class="mob-header" >
        <div class="nav-list">
           <div class="logo active-logo">
                <router-link to="/">
                <div><img src="../../assets/images/logo.svg" alt="img"/></div>
                <div class="logo-text"><span>Litekart</span></div>
              </router-link>
            </div>
         <button class="memu-icon" v-on:click="toggleMenu" >
           <svg fill="none" xmlns="http://www.w3.org/2000/svg" class="w-6 h-6 fill-current" data-v-705463ae=""><path fill-rule="evenodd" clip-rule="evenodd" d="M2 12a1 1 0 011-1h18a1 1 0 110 2H3a1 1 0 01-1-1zM2 6a1 1 0
              011-1h18a1 1 0 110 2H3a1 1 0 01-1-1zM2 18a1 1 0 011-1h18a1 1 0
              110 2H3a1 1 0 01-1-1z" data-v-705463ae=""></path></svg>
         </button>
      </div>
      <div class="mob-menu" v-if="mobileMenu">
          <div class="dropdown-menu">
            <div class="close-btn" v-on:click="toggleMenu">
            <svg data-v-705463ae="" fill="none" xmlns="http://www.w3.org/2000/svg" class="w-6 h-6 fill-current"><path data-v-705463ae="" fill-rule="evenodd" clip-rule="evenodd" d="M18.707 5.293a1 1 0 010 1.414l-12 12a1 1 0
                01-1.414-1.414l12-12a1 1 0 011.414 0z"></path> <path data-v-705463ae="" fill-rule="evenodd" clip-rule="evenodd" d="M5.293 5.293a1 1 0 011.414 0l12 12a1 1 0 01-1.414
                1.414l-12-12a1 1 0 010-1.414z"></path></svg>
          </div>
         <ul class="menu" v-on:click="toggleMenu">
                <li><router-link to="/">
                <svg data-v-705463ae="" fill="none" viewBox="0 0 24 24" stroke="currentColor" class="w-5 h-5 mr-2"><path data-v-705463ae="" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2
                  2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0
                  011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6"></path></svg>
                  HOME</router-link> </li>
                <li><router-link to="blog">
                  <svg data-v-705463ae="" fill="none" viewBox="0 0 24 24" stroke="currentColor" class="w-5 h-5 mr-2"><path data-v-705463ae="" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 5a1 1 0 011-1h14a1 1 0 011 1v2a1 1 0 01-1 1H5a1 1 0
                  01-1-1V5zM4 13a1 1 0 011-1h6a1 1 0 011 1v6a1 1 0 01-1 1H5a1
                  1 0 01-1-1v-6zM16 13a1 1 0 011-1h2a1 1 0 011 1v6a1 1 0 01-1
                  1h-2a1 1 0 01-1-1v-6z"></path></svg>
                  BLOG
                  </router-link> </li>
                <li><router-link to="/live-projects">
                <svg data-v-705463ae="" xmlns="http://www.w3.org/2000/svg" width="24px" height="24px" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 mr-2 feather feather-code"><polyline data-v-705463ae="" points="16 18 22 12 16 6"></polyline><polyline data-v-705463ae="" points="8 6 2 12 8 18"></polyline></svg>
                LIVE PROJECTS
                </router-link></li>
                <li><router-link to="features">
                  <svg data-v-705463ae="" xmlns="http://www.w3.org/2000/svg" width="24px" height="24px" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 mr-2 feather feather-upload-cloud"><polyline data-v-705463ae="" points="16 16 12 12 8 16"></polyline><line data-v-705463ae="" x1="12" y1="12" x2="12" y2="21"></line><path data-v-705463ae="" d="M20.39 18.39A5 5 0 0 0 18 9h-1.26A8 8 0 1 0 3 16.3"></path><polyline data-v-705463ae="" points="16 16 12 12 8 16"></polyline></svg>
                  FEATURES</router-link> </li>
                <li><router-link to="/litekart-story">
                <svg data-v-705463ae="" xmlns="http://www.w3.org/2000/svg" width="24px" height="24px" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 mr-2 feather feather-upload-cloud"><polyline data-v-705463ae="" points="16 16 12 12 8 16"></polyline><line data-v-705463ae="" x1="12" y1="12" x2="12" y2="21"></line><path data-v-705463ae="" d="M20.39 18.39A5 5 0 0 0 18 9h-1.26A8 8 0 1 0 3 16.3"></path><polyline data-v-705463ae="" points="16 16 12 12 8 16"></polyline></svg>
                STORY</router-link></li>
                <li><router-link to="/technology">
                <svg data-v-705463ae="" xmlns="http://www.w3.org/2000/svg" width="24px" height="24px" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 mr-2 feather feather-upload-cloud"><polyline data-v-705463ae="" points="16 16 12 12 8 16"></polyline><line data-v-705463ae="" x1="12" y1="12" x2="12" y2="21"></line><path data-v-705463ae="" d="M20.39 18.39A5 5 0 0 0 18 9h-1.26A8 8 0 1 0 3 16.3"></path><polyline data-v-705463ae="" points="16 16 12 12 8 16"></polyline></svg>
                TECHNOLOGY</router-link></li>
                <li><router-link to="/ecommerce-developer">
                <svg data-v-705463ae="" xmlns="http://www.w3.org/2000/svg" width="24px" height="24px" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 mr-2 feather feather-upload-cloud"><polyline data-v-705463ae="" points="16 16 12 12 8 16"></polyline><line data-v-705463ae="" x1="12" y1="12" x2="12" y2="21"></line><path data-v-705463ae="" d="M20.39 18.39A5 5 0 0 0 18 9h-1.26A8 8 0 1 0 3 16.3"></path><polyline data-v-705463ae="" points="16 16 12 12 8 16"></polyline></svg>
                DEVELOPERS</router-link></li>
                <li><router-link to="/pricing">
                <svg data-v-705463ae="" xmlns="http://www.w3.org/2000/svg" width="24px" height="24px" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 mr-2 feather feather-upload-cloud"><polyline data-v-705463ae="" points="16 16 12 12 8 16"></polyline><line data-v-705463ae="" x1="12" y1="12" x2="12" y2="21"></line><path data-v-705463ae="" d="M20.39 18.39A5 5 0 0 0 18 9h-1.26A8 8 0 1 0 3 16.3"></path><polyline data-v-705463ae="" points="16 16 12 12 8 16"></polyline></svg>
                PRICING</router-link></li>
                <li><router-link to="/contact">
                <svg data-v-705463ae="" xmlns="http://www.w3.org/2000/svg" width="24px" height="24px" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 mr-2 feather feather-upload-cloud"><polyline data-v-705463ae="" points="16 16 12 12 8 16"></polyline><line data-v-705463ae="" x1="12" y1="12" x2="12" y2="21"></line><path data-v-705463ae="" d="M20.39 18.39A5 5 0 0 0 18 9h-1.26A8 8 0 1 0 3 16.3"></path><polyline data-v-705463ae="" points="16 16 12 12 8 16"></polyline></svg>
                Contact Us</router-link></li>
        </ul>
          </div>
      </div>
    </div>
  
</div>
</template>

<script>
import DropDown from '@/components/header-dropdown/HeaderDropdown';
export default {
    name: 'AppHeader',
    components: {
      DropDown
    },
    data: function () {
     return {
       mobileMenu: false
     }
    },
    methods:{
      toggleMenu: function () {
        this.mobileMenu = !this.mobileMenu
      }
    }
};
</script>

<style scoped>

/* header start  */

.header-section{
    background-color: #fff;
    position: relative;
    z-index: 1;
    position: fixed;
    width:100%;
    top:0;
}
.since-primary{
    background-color: #000000;
    text-align: center;
    padding: 10px;
}
.since-primary h6{
    margin: 0;
    font-size: 13px;
    color: #fff;
    word-spacing: 1.5px;
    letter-spacing: 1.5px;
}
.header-primary{
    box-shadow: 0 1px 3px 0 rgba(0,0,0,.1), 0 1px 2px 0 rgba(0,0,0,.06);
    padding:20px 32px;
}
.header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
}
.header .primary-list{
    display: flex;
    align-items: center;
}
.header .active-logo .router-link-exact-active{
    background-size: 100% 5px!important;
    border-radius: unset!important;
}
.header .logo a{
    text-decoration: none;
    display: flex;
    align-items: center;
    padding:6px 0;
}
.header .logo img{
    height: 30px;
}
.header .logo a .logo-text{
    font-size: 26px;
    font-weight: bold;
    color: #282c3f;
    padding-left:5px;
}
.header .active-class .router-link-exact-active{
    background-image: linear-gradient(90deg,#fa709a 0,#fee140);
    background-repeat: no-repeat;
    background-size: 100% .2em;
    background-position: 0 100%;
    transition: background-size .25s ease-in;
    text-decoration: none;
    border-radius:8px;
}
.navigation-list>ul{
    display: flex;
    padding:2px 20px;
    margin:0 20px;
    border-left:1px solid #e2e8f0;
}
.navigation-list>ul li{
    list-style-type: none;
    margin: 0 6px;
    position: relative;
    border-radius: 8px;
     top:2px;
}
.navigation-list>ul>li>a{
    text-decoration: none;
    color: #282c3f;
    font-size: 15px;
    display: block;
    padding:5px 14px;
}
.navigation-list>ul>li>a:after {
    content: "";
    width: 0;
    height: 3px;
    display: block;
    position: relative;
    top:5px;
    background-image: linear-gradient(90deg,#fa709a 0,#fee140);
    background-repeat: no-repeat;
    transition: width .2s ease;
    -webkit-transition: width .2s ease;
}
.navigation-list>ul>li>a:hover:after{
    width: 100%;
}
.lets-talk{
    display: flex;
    align-items: center;
}
.lets-talk .btn-talk{
    background-color: #3182CE;
    color:#fff;
    box-shadow: 1px 1px 3px 0 rgba(8,116,249,.4);
}
.lets-talk .price-list ul{
    border-left:unset;
}
.lets-talk .talk-btn:hover{
    transition-duration: .5s;
    background-color: #4299e1;
}
.dropdown-head{
   display: none;
}
.hover-dropdown:hover .dropdown-head {
    display: block;
}
/* header end */
.mob-header{
  display: none;
}
@media (max-width: 479px) and (min-width: 320px) {
  
    .hero-container {
        padding: 30px;
    }
    .hero-container .hero {
        flex-wrap: wrap;
    }
    .hero-container .hero .hero-left {
        padding: 0px;
        width: 100%;
    }
    .hero-container .hero .hero-left h2 {
        font-size: 36px;
    }
    .discount-btn {
        margin-left: 0px;
    }
    .hero-container .hero .hero-right {
        display: none;
    }
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
    .since-primary h6{
      font-size: 10px;
    }

    /* Mobile menu Responsive css */
  .header-primary{
    display: none;
  }
.close-btn{
 float: right;
}
.close-btn svg{
  width: 30px;
  height: 30px;
  color: #000000;
  fill: currentColor;
  background-color: #f7fafc;
  border: 1px solid  #f7fafc;
}
.mob-header{
  display: block;
 position: fixed;
 z-index: 1;
 top: 31px;
 width: 100%;
 background-color: #fff;
 box-shadow: 0 1px 3px 0 rgba(0,0,0,.1), 0 1px 2px 0 rgba(0,0,0,.06);
}
.dropdown-menu{
  width: 290px;
  list-style: none;
  background-color: #fff;
  height: 100vh;
  padding: 4rem 40px 20px 20px;
}
.nav-list{
  display: flex;
 justify-content: space-between;
 padding: 20px;
 align-items: center;
}
.memu-icon{
border-radius: .25rem;
background-color: #f7fafc;
cursor: pointer;
border: none;
padding: 6px 8px;
}
.memu-icon svg{
      width: 24px;
      fill: currentColor;
      height: 24px;
}
 .active-logo .router-link-exact-active{
    background-size: 100% 5px!important;
    border-radius: unset!important;
}
 .logo a{
    text-decoration: none;
    display: flex;
    align-items: center;
    padding:6px 0;
}
.logo img{
    height: 30px;
}
.logo a .logo-text{
    font-size: 26px;
    font-weight: bold;
    color: #282c3f;
    padding-left:5px;
}
.active-class .router-link-exact-active{
    background-image: linear-gradient(90deg,#fa709a 0,#fee140);
    background-repeat: no-repeat;
    background-size: 100% .2em;
    background-position: 0 100%;
    transition: background-size .25s ease-in;
    text-decoration: none;
    border-radius:8px;
}
.mob-menu{
    display: flex;
    justify-content: flex-end;
    position: fixed;
    right: 0;
    top: 0;
}
.mob-menu .menu{
  list-style: none;
  padding: 0px;
  margin-top: 5rem;
}
.mob-menu .menu>li{
  margin-bottom: 1.5rem;
}
.mob-menu .menu>li>a{
    text-decoration: none;
    color: #282c3f;
    font-size: 18px;
    display: flex;
    align-items: center;
    padding:5px 14px;
    
}
.mob-menu .menu>li>a svg{
  width: 24px;
  height: 24px;
  margin-right: 10px;
}
}

@media (max-width: 684px) and (min-width: 575px) {}

@media (max-width: 767px) and (min-width: 685px) {}

@media (max-width: 991px) and (min-width: 768px) {}

@media (max-width: 574px) and (min-width: 480px) {}

@media (max-width: 1199px) and (min-width: 1024px) {}

</style>