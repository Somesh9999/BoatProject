<template>
  <section class="bgboat">
    <div class="wrapper">
      <div class="col-1-2">
        <div class="product-wrap">
          <div class="product-shot">
            <img src="../assets/boat1.jpg" alt="" />
          </div>
        </div>
      </div>

      <div class="col-1-2">
        <div class="product-info">
          <h2>Tourist speed boat for sightseeing at Andaman sea</h2>
          <div class="desc"></div>
          <ul>
            <li>Boat Name: <b>Stussy</b></li>
            <li>Type:</li>
            <li>No Of Rooms: 4</li>
            <li>No Of Bedrooms: 4</li>
            <li>Cost Per Night: Rs. 250.00</li>
            <li>Image URL:</li>
            <!-- <li>
              Classification: From its humble origins as a surfwear brand,
              Stussy has gone on to become one of the biggest streetwear labels
              in the industry. Mixing various influences ranging from surf to
              music and everything in between, Stussy and it’s iconic signature
              graphic has grown to encapsulate a full range of apparel, home
              goods and limited-edition collaborations. 100% premium cotton
              raglan tee with 3/4 -length contrasting sleeves and graphic print
              on chest.
            </li> -->
          </ul>
          <!-- <ul class="sizing-list">
              <li class="size">S</li>
              <li class="size active">M</li>
              <li class="size">L</li>
            </ul> -->
          <button class="button"> Edit </button>
        </div>
      </div>
    </div>
  </section>
</template>    
    
          <script>
document.body.addEventListener("click", function (event) {
  event.target.classList.toggle("active");
});
</script>


      <style scoped>
img {
  max-width: 100%;
  height: 268px;
}

.wrapper {
  width: 960px;
  margin: 100px auto;
}

.col-1-2 {
  float: left;
  width: 50%;
}

.product-wrap {
  margin: 0 auto;
  width: 350px;
}
.product-wrap .product-shot {
  padding-top: 60px;
  transition: all 0.5s ease;
}
.product-wrap .product-shot:hover {
  transform: scale(1.1);
}

.product-info h2 {
  padding-bottom: 15px;
  font-size: 32px;
  border-bottom: 1px solid #d9d9d9;
}
.product-info .desc {
  margin-top: 25px;
  font-size: 16px;
  line-height: 1.6;
}
.product-info .sizing-list {
  margin-top: 25px;
  padding: 0px;
  list-style-type: none;
}
.product-info .size {
  display: inline;
  margin-right: 10px;
  padding: 10px 15px;
  color: #c2c2c2;
  border: 1px solid #c2c2c2;
  cursor: pointer;
}
.product-info .size.active {
  color: white;
  background-color: #c2c2c2;
}

.button {
  display: inline-block;
      background-image: linear-gradient(to right, #1a2980, #26d0ce);
          background-image: linear-gradient(to right, #1a2980, #26d0ce);
    border-radius: 20px;
    height: 35px;
    line-height: 35px;
    width: 26%;
    border: none;
    outline: none;
    cursor: pointer;
    color: #fff;
    font-size: 1.1em;
    margin: 20px;
    transition: all 0.3s ease-in-out;
}

.button:hover {
  background-color: #323232;
}
.bgboat{
    background-image: url('../assets/bgsea.jpg');
}
</style>
    


    