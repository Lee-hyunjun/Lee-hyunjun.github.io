<template>
  <div class="Navs">
    <div>
      <img src="../assets/logo.png" alt="Logo">
      <div>
        <p>About</p> 
        <p>Business</p> 
        <p>area</p> 
        <p>Target</p> 
        <p>Our goal</p> 
        <p>Works</p> 
        <p>Partners</p> 
        <p>Contact</p> 
      </div>
    </div>
  </div>
</template>

<script>

// import Logo from "@/assets/logo.png"

export default {
  components: {
    // Logo
  }
}
</script>

<style  lang="scss">
  .Navs{
    position: absolute;
    top: 55px;
    width: 100%;

    >div{
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      width: 100%;
      margin: 0 auto;


      >div{
        display: flex; 
        align-items: center;

        p{
          color: white;
          margin-left: 24px;
          position: relative;
          transition: .3s;
          font-family: 'Objektiv Mk2 W03 Medium' ,sans-serif;
          font-size: .875rem;
        }



        p:hover{
          cursor: pointer;
        }

        p::after{
          content: "";
          opacity: 0;
        }

        p:hover::after{
          content: "";
          width: 100%;
          opacity: 1;
          height: 1px;
          position: absolute;
          bottom: 0;
          left: 0;
          background:white;
          -webkit-transition: all .3s;
          transition: all .3s;
        }
      }
    }
  }
</style>
