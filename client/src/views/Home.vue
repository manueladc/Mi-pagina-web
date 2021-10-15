<template>
  <BasicLayouts>
</BasicLayouts>


            <div class="banner">
              
            </div>

      
         <div class="services">
             <h1>M y E Beauty</h1>
        </div>

        <section  class="services-section">

           
          
            <article >
                

                <router-link class="item" to="/skincare" > 
                  <img  src="../assets/antenas.jpg" alt="skincare" >
                 </router-link>  
                    <h2 >Skincare</h2>
                 
            </article>

            <article >
               <router-link class="item" to="/maquillaje" > 
                <img  src="../assets/maquillaje.jpg" alt="maquillaje">
                </router-link> 
                <h2 >Maquillaje</h2>
                
            </article>

            <article class="item">

              <router-link class="item" to="accesorios" > 
                <img  src="../assets/accesorios.jpg" alt="accesorios" >
                </router-link> 

                <h2 >Accesorios</h2>
                
            </article>

        </section>
       

    

    
    

  <footer class="footer">

        <article>
           <p>Copyright © 2021 M y E Beauty Todos los derechos reservados.</p>
        </article> 
    </footer>  
 
  
</template>



<script>
import { ref, onMounted } from 'vue';
import{useRouter }from 'vue-router';
import BasicLayouts from '../layouts/BasicLayouts.vue';
import{}from '../api/category';


export default {
  name: 'Inicio',
  components: {
    BasicLayouts,
    
  }
  
};

</script>

<style scoped>



.banner {
  width: 100%;
  height: 500px;
  max-width: 100%;
  object-fit: cover;
  display: block;
  margin: auto;
  background-size: cover;
  background-size: 100% 100%;
  animation: banner 20s infinite;
  animation-direction:alternate;
  background-image: url("../assets/banner1.jpg");
}

/* @keyframes banner{
  0%, 30% {
    background-image: url("../assets/banner1.jpg");
  }

  31%,34%{
    opacity:0.1;
  }
  35%, 65% {
    background-image: url("../assets/banner2.jpg");
    opacity: 1;
  }
  66%,69%{
    opacity: 0.1;
  }
   70%, 100% {
     opacity: 1;
    background-image: url("../assets/banner3.jpg");
  }
} */

.services{
  /*background-color: #3689d6;*/
  background-image: url('../assets/header1.jpg');
  height: 100px;
  color: white;
  /*Para centrar un contenido*/
  display: flex;
  justify-content: center;
  align-items: center;
  
}

.header-container {
  background-color: #a333ff;
}
.services-section {
  display: flex;
  align-items: center; 
  
}

.services-section article {
  padding: 20px;
  text-align: center;
}

.services-section img {
  border-radius: 60%;
  margin-right: auto;
  margin-left: auto;
  width: 60%;
  height: 60%;
  margin-bottom: 30px;
}

.domotica{
   margin-bottom: 10px;
}
.services-section p {
  font-size: 20px;
  text-align:center;
  
}

.footer {
  background-color: #ff3396;
  height: 150px;
  display: flex;
  color: white;
  justify-content: space-evenly;
}

footer p {
  font-size: 20px;
}

</style>