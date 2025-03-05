<template>
    <header>
        <img src="/assets/images/Hero_image.jpg" alt="" height="1280" width="855">
    <div> test</div>
    </header>
</template>


<style lang="scss" scoped>
//mobile
    header {
      img {
        width: 100%;
        height: 145px;
        object-fit: cover;
        object-position: 0% 35%; 
        }
         div{
        background-color: red;
        }
   
    }

    // tablet
    @media screen and (min-width: 768px) { 
        header {
            img {
             width: 100%; 
             height: 445px;
             object-fit: cover;
             object-position: 0% 0%; 
          }
         div{
        background-color: aqua;
        }
        
        }
    }

    //desktop
     @media screen and (min-width: 1024px) { 
     header{
        img{
            width: 100%; 
            height: 690px;
            object-fit: cover;
            object-position: 0% 30%; 
        }
        div{
        background-color: brown;
        }
    }
    }

</style>