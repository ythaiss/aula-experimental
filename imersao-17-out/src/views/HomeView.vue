<script setup lang="ts">
import Logo from "../assets/img/logo/Frame 57.png"
import BannerImg from '../assets/img/banner/banner-main.png'
import TarjaImgWhite from '@/assets/img/banner/bannerwhite.jpeg'
import TarjaImgYellow from '../assets/img/banner/banneryellow.jpeg'
</script>

<template>
  <main>
     <header>
        <div class="logo">
          <img :src="Logo" alt="">
        </div>
        <nav>
          <ul>
            <li>CATALOGUE</li>
            <li>FASHION</li>
            <li>FAVORITE</li>
            <li>LIFESTYLE</li>
          </ul>
          <button>
              SIGN UP
          </button>
        </nav>
     </header>
     <section class="banner">
        <div class="text">
           <div class="tarja">
              <!-- <img :src="TarjaImgWhite" alt=""> -->
              <img :src="TarjaImgYelllow" alt="">
          </div>
           <h1> LET'S<br/>
                EXPLORE<br/> 
                UNIQUE<br/> 
                CLOTHES
            </h1>
       
        </div>
        <div class="img">
          <img :src="BannerImg" alt="">
        </div>
     </section>
  </main>
</template>
<style scoped>
main{
    width: 1290px;
    margin: 0 auto;
}   
main header{
    display: flex;
    justify-content: space-between;
}
main .banner{
    margin: 30px 0 0 0;
    display: flex;
    justify-content: space-between;
    background-color: #F4F6F5;
    border-radius: 59px;
    padding: 70px 70px 0 30px;
}
main .banner .text{
    position: relative;
}
main .banner .text .tarja{
    position: absolute;
    z-index: 0;
}
main .banner .text .tarja img:first-child{
    width: 400px;
    left: -20px;
    position: absolute;
    z-index: 0;
}
main .banner .text .tarja img:nth-last-of-type(2){
    width: 400px;
    left: -20px;
    position: absolute;
    z-index: 0;
    top: 240px;
}
main .banner .text h1{
    font-weight: 900;
    font-size: 80px;
    padding: 0;
    margin: 0;
}
main .banner .img{
    width: 55%;
}
main .banner .img img{
    width: 100%;
}
main header nav{
    display: flex;
    align-items: center;
    gap: 15px;

}
main header nav ul{
    padding: 0;
    display: flex;
    gap: 35px;

}
main header nav ul li{
    list-style: none;
    padding: 0;
    font-size: 18px ;

}
main header nav button{
    padding: 8px 12px;
    background-color: black;
    border-radius: 4px;
    cursor: pointer;
    color: white;

}

</style>
