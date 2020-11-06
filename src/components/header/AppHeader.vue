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

    <div class="mob-header">
        <div class="logo active-logo">
        <router-link to="/">
        <div><img src="../../assets/images/logo.svg" /></div>
        <div class="logo-text"><span>Litekart</span></div>
      </router-link>
    </div>
        <div id="menuToggle">  
        <input type="checkbox" />
        <span></span>
        <span></span>
        <span></span>
        <ul id="menu">
          <a href="#"><li>Home</li></a>
          <a href="#"><li>About</li></a>
          <a href="#"><li>Info</li></a>
          <a href="#"><li>Contact</li></a>
          <a href="#" target="_blank"><li>Show me more</li></a>
        </ul>
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
#menuToggle{
  display: none;
}

@media (max-width: 479px) and (min-width: 320px) {
  .header-primary{
  display: none;
  }
  .header-section{
    position: unset;
  }
  .mob-header{
   position: relative;
   top: 50px;
   left: 0px;
   width: 100%;
  }
   .logo a{
    text-decoration: none;
    display: flex;
    align-items: center;
    padding:6px 0;
   }
  .logo a>div img{
  height: 30px;
  margin-right: 10px;
  }
  #menuToggle{
  display: block;
  position: relative;
  top: 50px;
  left: 50px;
  z-index: 1;
  user-select: none;
}

#menuToggle a
{
  text-decoration: none;
  color: #232323;
  transition: color 0.3s ease;
}

#menuToggle a:hover
{
  color: tomato;
}


#menuToggle input
{
  display: block;
  width: 40px;
  height: 32px;
  position: absolute;
  top: -7px;
  left: -5px;
  cursor: pointer;
  opacity: 0; /* hide this */
  z-index: 2; /* and place it over the hamburger */
  -webkit-touch-callout: none;
}

/*
 * Just a quick hamburger
 */
#menuToggle span
{
  display: block;
  width: 33px;
  height: 4px;
  margin-bottom: 5px;
  position: relative;
  
  background: #cdcdcd;
  border-radius: 3px;
  
  z-index: 1;
  
  transform-origin: 4px 0px;
  
  transition: transform 0.5s cubic-bezier(0.77,0.2,0.05,1.0),
              background 0.5s cubic-bezier(0.77,0.2,0.05,1.0),
              opacity 0.55s ease;
}

#menuToggle span:first-child
{
  transform-origin: 0% 0%;
}

#menuToggle span:nth-last-child(2)
{
  transform-origin: 0% 100%;
}

/* 
 * Transform all the slices of hamburger
 * into a crossmark.
 */
#menuToggle input:checked ~ span
{
  opacity: 1;
  transform: rotate(45deg) translate(-2px, -1px);
  background: #232323;
}

/*
 * But let's hide the middle one.
 */
#menuToggle input:checked ~ span:nth-last-child(3)
{
  opacity: 0;
  transform: rotate(0deg) scale(0.2, 0.2);
}

/*
 * Ohyeah and the last one should go the other direction
 */
#menuToggle input:checked ~ span:nth-last-child(2)
{
  transform: rotate(-45deg) translate(0, -1px);
}

/*
 * Make this absolute positioned
 * at the top left of the screen
 */
#menu
{
  position: absolute;
  width: 300px;
  margin: -100px 0 0 -50px;
  padding: 50px;
  padding-top: 125px;
  
  background: #ededed;
  list-style-type: none;
  -webkit-font-smoothing: antialiased;
  /* to stop flickering of text in safari */
  
  transform-origin: 0% 0%;
  transform: translate(-100%, 0);
  
  transition: transform 0.5s cubic-bezier(0.77,0.2,0.05,1.0);
}

#menu li
{
  padding: 10px 0;
  font-size: 22px;
}

/*
 * And let's slide it in from the left
 */
#menuToggle input:checked ~ ul
{
  transform: none;
}

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
}

@media (max-width: 684px) and (min-width: 575px) {}

@media (max-width: 767px) and (min-width: 685px) {}

@media (max-width: 991px) and (min-width: 768px) {}

@media (max-width: 574px) and (min-width: 480px) {}

@media (max-width: 1199px) and (min-width: 1024px) {}

</style>