<template>
  <div class="inicio">
    <div class="header mb-5 text">
      <b-navbar toggleable="lg">
      
      <img class="navbar-logo" src="../assets/logo-ccat.png">

      <b-navbar-brand href="#" class="text-white" >CENTRO CULTURAL AVANZADA TECNOLOGICA</b-navbar-brand>

     <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
     
      <!-- Right aligned nav items -->
       <b-navbar-nav class="ml-auto">
         <b-nav-item link-classes="text-white">Inicio</b-nav-item>
         <b-nav-item-dropdown toggle-class="text-white" text="¿Quiénes somos" right >
          <b-dropdown-item href="#">Nosotros</b-dropdown-item>
          <b-dropdown-item href="#">Miembros</b-dropdown-item>    
         </b-nav-item-dropdown>

           <b-nav-item-dropdown toggle-class="text-white" text="Áreas" right >
             <b-dropdown-item href="#">Direcciones</b-dropdown-item>
             <b-dropdown-item href="#">Gerencias</b-dropdown-item>    
           </b-nav-item-dropdown>

          <b-nav-item-dropdown toggle-class="text-white" text="Proyectos" droprightright >
            <b-dropdown-item   href="#">Proyectos</b-dropdown-item>
            <b-dropdown-item   href="#">Competitividad</b-dropdown-item>
            <b-dropdown-item   href="#">CODEX</b-dropdown-item>
          </b-nav-item-dropdown>

          <b-nav-item link-classes="text-white">Productos</b-nav-item>
          <b-nav-item link-classes="text-white">Próximos eventos</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
      </b-navbar>
    </div>

    <div class="carousel-inicio mb-5">
      <b-container>
        <b-carousel
            id="carousel-fade"
            style="text-shadow: 0px 0px 2px #000"
            fade
            controls
            indicators
            img-width="1024"
            img-height="480"
         >
            <b-carousel-slide
                  caption="First slide"
                  img-src="https://picsum.photos/1024/480/?image=10"
            ></b-carousel-slide>
            <b-carousel-slide
                  caption="Second Slide"
                  img-src="https://picsum.photos/1024/480/?image=12"
            ></b-carousel-slide>
            <b-carousel-slide
                  caption="Third Slide"
                  img-src="https://picsum.photos/1024/480/?image=22"
            ></b-carousel-slide>
      
        </b-carousel>
      </b-container>
    </div>

    <div class="convenios mb-5 mt-4">
      <b-container>
        <h1 class="text-center mb-5">CONVENIOS</h1>
        <b-row cols="2">
          <b-col>
            <h2 class= "text-center mb-4">AUSPICIADORES</h2>
              <div id="app">
                <vue-glide>
                    <vue-glide-slide >
                      <img class="slide-logo" src="../assets/ainad-logo.png" alt="">
                    </vue-glide-slide>
                    <vue-glide-slide>
                      <img class="slide-logo" src="../assets/fiis-logo.jpg" alt="">
                    </vue-glide-slide>
                    <vue-glide-slide>
                      <img class="slide-logo" src="../assets/nucleo-logo.png" alt="">
                    </vue-glide-slide>
                    <vue-glide-slide>
                      <img class="slide-logo" src="../assets/proyecta-logo.jpg" alt="">
                    </vue-glide-slide>

                    <vue-glide-slide>
                      <img class="slide-logo" src="../assets/dmc-logo.png" alt="">
                    </vue-glide-slide>
                  
              </vue-glide>
              </div>
           
          </b-col>

          <b-col>
            <h2 class= "text-center mb-4">ALIADOS</h2>
            <div id="app">
                <vue-glide>
                    <vue-glide-slide >
                      <img class="slide-logo" src="../assets/ainad-logo.png" alt="">
                    </vue-glide-slide>
                    <vue-glide-slide>
                      <img class="slide-logo" src="../assets/fiis-logo.jpg" alt="">
                    </vue-glide-slide>
                    <vue-glide-slide>
                      <img class="slide-logo" src="../assets/nucleo-logo.png" alt="">
                    </vue-glide-slide>
                    <vue-glide-slide>
                      <img class="slide-logo" src="../assets/proyecta-logo.jpg" alt="">
                    </vue-glide-slide>
                     <vue-glide-slide>
                      <img class="slide-logo" src="../assets/dmc-logo.png" alt="">
                    </vue-glide-slide>
                  
              </vue-glide>
              </div>
          </b-col>
          
        </b-row>
      </b-container>
    </div>
    
    <div class="footer-inicio mt-5">
      <b-row cols="3">
        <b-col>
          <b-container>
          <p class="imagen-centrado-texto">
          <img class="footer-logo" src="../assets/logo-ccat.png">
          </p>
           <p class="mt-3 text-center text-white mb-4">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt. 
           </p> 
          <h5 class="text-left text-white mt-4">Redes Sociales</h5>
          
          </b-container>
        </b-col>

      </b-row>
      
    </div>

  </div>
</template>


<script>
import { Glide, GlideSlide } from 'vue-glide-js'
  export default {
    name: 'HelloWorld',
    components: {
    [Glide.name]: Glide,
    [GlideSlide.name]: GlideSlide
  }
  }
</script>


<style>

  .navbar-logo{
     width:80px;
     height:80px;
     margin-right:10px;
  }

  .header{
    background-color: rgb(0,0,36,255);
  }
  
  .slide-logo{
    width:80px;
    height:80px;
  }

  .footer-logo{
    width:80px;
    height:80px;
    
  }

  .footer-inicio{
    background-color: rgb(0,0,36,255);
  }

  .imagen-centrado-texto{
    text-align: center;
    margin-top: 50px;
  }

</style>
