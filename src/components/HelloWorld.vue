<template>

      <div class="container ">
        <div class="row">
            
          <div class="topPic col-lg-4 col-md-4 col-sm-6">
              <!-- <img class="picture" width="350" height="300" src="images/center.jpeg"  alt="pic" > -->
          <img id="image1" class="image  " :src="render1"  height="300" alt="">

          </div>
          <div class="topPic col-lg-4 col-md-4 col-sm-6">
              <!-- <img class="picture" width="350" height="300" src="../assets/cityRain.jpeg"  alt="pic" > -->
          <img id="image2" class="image" :src="render2"  height="300" alt="">

          </div>
          <div class="topPic col-lg-4 col-md-4 col-sm-6">
              <!-- <img class="picture" width="350" height="300" src="../assets/face.jpeg"  alt="pic" > -->
          <img id="image3" class="image" :src="render3" height="300" alt="">

          </div>
          <div class="topPic col-lg-4 col-md-4 col-sm-6">
              <!-- <img class="picture" width="350" height="300" src="../assets/nightCity.jpeg"  alt="pic" > -->
          <img id="image4" class="image" :src="render4"  height="300" alt="">

          </div>
          <div class="topPic col-lg-4 col-md-4 col-sm-6">
              <!-- <img class="picture" width="350" height="300" src="../assets/center.jpeg"  alt="pic" > -->
          <img id="image5" class="image" :src="render5"  height="300" alt="">

          </div>
          <div class="topPic col-lg-4 col-md-4 col-sm-6">
              <!-- <img class="picture" width="350" height="300" src="../assets/logo.png"  alt="pic" > -->
          <img id="image6" class="image" :src="render6"  height="300" alt="">

          </div>
          <div class="topPic col-lg-4 col-md-4 col-sm-6">
              <!-- <img class="picture" width="350" height="300" src="../assets/logo.png"  alt="pic" > -->
          <img id="image7" class="image" :src="render7"  height="300" alt="">

          </div>
          <div class="topPic col-lg-4 col-md-4 col-sm-6">
              <!-- <img class="picture" width="350" height="300" src="../assets/logo.png"  alt="pic" > -->
          <img id="image8" class="image" :src="render8" height="300" alt="">

          </div>

          </div>
        </div>


</template>

<script>


    export default {
        data() {

            return {
                render1:null, 
                render2:null,
                render3:null,
                render4:null,
                render5:null,
                render6:null, 
                render7:null, 
                render8:null, 
                images:[]
            }
            
        },
        created(){        
            let self = this;
             let images = [{image:"images/center.jpeg"}, {image:"images/cityRain.jpeg"}, { image:"images/nightCity.jpeg"},{ image:"images/12.jpeg"},{ image:"images/code.jpeg"},{ image:"images/codingImg.jpeg"},{ image:"images/highway.jpeg"},{ image:"images/temple.jpeg"},{ image:"images/waterFall.jpeg"}];
            
            setInterval(function() {
                self.render1 = images[Math.floor(Math.random() * images.length)].image;
                console.log(self.render1);
                // self.eddie = "images/cityRain.jpeg";
            },3000);
            setInterval(function() {
                self.render2 = images[Math.floor(Math.random() * images.length)].image;
                console.log(self.render2);
                // self.eddie = "images/cityRain.jpeg";
            },3500);
            setInterval(function() {
                self.render3 = images[Math.floor(Math.random() * images.length)].image;
                console.log(self.render3);
                // self.eddie = "images/cityRain.jpeg";
            },4500);
            setInterval(function() {
                self.render4 = images[Math.floor(Math.random() * images.length)].image;
                console.log(self.render4);
                // self.eddie = "images/cityRain.jpeg";
            },5500);   
            setInterval(function() {
                self.render5 = images[Math.floor(Math.random() * images.length)].image;
                console.log(self.render5);
                // self.eddie = "images/cityRain.jpeg";
            },4500);            
            setInterval(function() {
                self.render6 = images[Math.floor(Math.random() * images.length)].image;
                console.log(self.render6);
                // self.eddie = "images/cityRain.jpeg";
            },5500);
            setInterval(function() {
                self.render7 = images[Math.floor(Math.random() * images.length)].image;
                console.log(self.render7);
                // self.eddie = "images/cityRain.jpeg";
            },3500);
            setInterval(function() {
                self.render8 = images[Math.floor(Math.random() * images.length)].image;
                console.log(self.render8);
                // self.eddie = "images/cityRain.jpeg";
            },2000);
            
            

        }
    }

</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.container{
  background-color: rgba(7, 1, 1, 0.947);
  width: 100%;
  height: 100%;
  margin-left: 2%;
  margin-right: 2%;
  padding-top: 2%;

}

.topPic{
    float: left;
    background-color: black;
    width: 350px;
}
.image{
    width: 340px;
}


</style>
