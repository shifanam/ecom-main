<template>
  <div class="row">
    <div class="col-xs-12 col-sm-12 col-lg-12 col-md-12">
      <div class="row">
        <div class="col-xs-12 col-sm-12 col-lg-12 col-md-12">
          <div id="myCarousel" class="carousel slide" data-ride="carousel">
            <!-- Indicators -->
            <ol class="carousel-indicators">
              <li data-target="#myCarousel" data-slide-to="0" class="active"></li>
              <li data-target="#myCarousel" data-slide-to="1"></li>
              <li data-target="#myCarousel" data-slide-to="2"></li>
            </ol>
            <!-- Wrapper for slides -->
            <div class="carousel-inner">
              <div class="item active">
                <img src="../assets/slider1.jpg" alt="Los Angeles" style="width:100%; height:400px;">
                <div class="carousel-caption">
                  <h3>Los Angeles</h3>
                  <p>LA is always so much fun!</p>
                </div>
              </div>
              <div class="item">
                <img src="../assets/slide.png" alt="Los Angeles" style="width:100%; height:400px;">
                <div class="carousel-caption">
                  <h3>Los Angeles</h3>
                  <p>LA is always so much fun!</p>
                </div>
              </div>
              <div class="item">
                <img src="../assets/slider5.jpg" alt="Los Angeles" style="width:100%; height:400px;">
                <div class="carousel-caption">
                  <h3>Los Angeles</h3>
                  <p>LA is always so much fun!</p>
                </div>
              </div>
            </div>
            <!-- Left and right controls -->
            <a class="left carousel-control" href="#myCarousel" data-slide="prev">
              <span class="glyphicon glyphicon-chevron-left"></span>
              <span class="sr-only">Previous</span>
            </a>
            <a class="right carousel-control" href="#myCarousel" data-slide="next">
              <span class="glyphicon glyphicon-chevron-right"></span>
              <span class="sr-only">Next</span>
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
