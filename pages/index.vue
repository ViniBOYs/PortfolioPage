<script setup>
  import { DoorOpen } from 'lucide-vue-next';
  import { Search } from 'lucide-vue-next';
  import { Send } from 'lucide-vue-next';
  import { NotebookText } from 'lucide-vue-next';
</script>



<template>
    
        <div class="header"></div>
        <header>
        <nav>
          <ul>
            <li><DoorOpen/><a href="#">Home</a></li>
            <li><NotebookText /><a href="#">About</a></li>
            <li><Send/><a href="#">Contact</a></li>
          </ul>
        </nav>
        </header>    


        <section class="sec-1">

            <div class="circle">
                <div class="dot-circle">
                  <div class="title">
                    <h2>Be</h2>
                    <h1>Unique</h1>
                  </div>

                </div>
            </div>

            <div class="pyramid-loader">
            <div class="wrapper">
                <span class="side side1"></span>
                <span class="side side2"></span>
                <span class="side side3"></span>
                <span class="side side4"></span>
                <span class="shadow"></span>
            </div>  
            </div>
            
            
            <div class="socialLinks">
                <linkedin-component/>
                <GithubComponent/>
            </div>
    
        </section> <!-- Fim Sec-1 -->
        

        
        <!-- sec-2 -->
        <div class="black-bar"></div>
        <section class="sec-2">
            <div class="card">
            <b>
                <PiramedeQueGira/>
            </b>
            </div>
        </section>
        <div class="black-bar"></div>
        <!-- sec-2 -->




</template> 

<style scoped lang="scss">

.header{
  height: 2vw;
  background-color: #49333b;
}

header{
  position:sticky;
  height: 3vw;
  background-color: #49333b;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  // filter: blur(30px);
  z-index: 2;
  position: sticky;
  top: 0;
  box-shadow: 0 10px 20px #49333b;
  // rgba(73, 51, 59, 0.25);
  

  nav ul{
    // background-color: rgba(255, 255, 255, 0.171);
    display: flex;    
    
  }

  li{
    color: white;
    display: flex;
    padding: 0 10px 0;
  
    a{
      padding: 3px;
      color: #ffffff;
      text-decoration: none;
      text-transform: uppercase;
      font-family:Arial, Helvetica, sans-serif;
      font-weight: bold;
    }

  }



}




.sec-1{
    padding: 4vh;
    background-color: #1c1b1b;
    height: 90vh;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    align-content: center;
    place-items: center;


    h1 {
        color: #ffffff;
    }
}




.socialLinks{
    // background-color: #ffffff;
    width: 20vh;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-content: center;
    position: absolute;
    top: 87vh;
    left: 177vh;
}




.dot-circle {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
  width: 40vw;
  height: 40vw;
  background-image: radial-gradient(rgba(255, 255, 255, 0.171) 2px, transparent 0);
  background-size: 30px 30px;
  background-position: -5px -5px;
  border-radius: 20vw;
  
  .title{
    // background-color: rgba($color: #44aa22, $alpha: .2);
    position: relative;
    // left: -10vw;

      
    h2{
      // background-color: rgba($color: #ffaaff, $alpha: .2);
      color: orange;
      font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
      font-size: 90px;
      text-shadow: 5px 5px 10px #03a9f4,
                  -5px -5px 10px #ff0058;
      
    }

    h1{
      // background-color: rgba($color: #ffffff, $alpha: .2);
      color: orange;
      font-family:'Times New Roman', Times, serif;
      font-size: 90px;
      text-shadow: 5px 5px 10px #03a9f4,
                  -5px -5px 10px #ff0058;
      
    }


  }
  
}








.sec-2 {
  height: 30vw;
  display: flex;
  padding-left:3vw;
  justify-content: start;
  align-items: center;

  /* Dark mode colors and gradient */
  background: #1c1b1b; /* Fallback for browsers that don't support gradients */
  background: linear-gradient(
    135deg,
    #1c1b1b 25%,
    #0d0d0d 25%,
    #0d0d0d 50%,
    #1c1b1b 50%,
    #1c1b1b 75%,
    #0d0d0d 75%,
    #0d0d0d
  );
  background-size: 40px 40px;

  /* Animation */
  animation: move 4s linear infinite;
}

.black-bar{
    height: 1vw;
    background-color: #0d0d0d;
}














</style>