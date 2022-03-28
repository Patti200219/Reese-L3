---
layout: layout.html
title: Photography
eleventyNavigation: 
 key: Photography 
---
<div class="TitleDiv">

# {{ title }} 
    
### Click the dots to see some of my works!

</div>


<!-- Slideshow container -->
<div class="slideshow-container">

  <!-- Full-width images with number and caption text -->
  <div class="mySlides fade">
    <div class="numbertext"></div>
    <img src="img/photography1.jpg" style="width:100%">
    <div class="text">Groggy Day At The Hospital: Red Lake Ontario</div>
  </div>

  <div class="mySlides fade">
    <div class="numbertext"></div>
    <img src="img/photography2.jpg" style="width:100%">
    <div class="text">Perrault Lake: Perrault Falls Ontario</div>
  </div>

  
  <div class="mySlides fade">
    <div class="numbertext"></div>
    <img src="img/photography3.jpg" style="width:100%">
    <div class="text">Howey Bay: Red Lake Ontario</div>
  </div>
  <div class="mySlides fade">
    <div class="numbertext"></div>
    <img src="img/photography4.jpg" style="width:100%">
    <div class="text">Portraits demo (serious)</div>
  </div>  

  <div class="mySlides fade">
    <div class="numbertext"></div>
    <img src="img/photography5.jpg" style="width:100%">
    <div class="text">Close Up Of Flowers: Red Lake Ontario</div>
  </div> 

  <div class="mySlides fade">
    <div class="numbertext"></div>
    <img src="img/photography6.jpg" style="width:100%">
    <div class="text">Roses Close Up: Red Lake Ontario</div>
  </div> 
  
  <div class="mySlides fade">
    <div class="numbertext"></div>
    <img src="img/photography7.jpg" style="width:100%">
    <div class="text">Portraits demo (silly)</div>
  </div> 

  <div class="mySlides fade">
    <div class="numbertext"></div>
    <img src="img/photography8.jpg" style="width:100%">
    <div class="text">Norseman Plane: Red Lake Ontario</div>
  </div> 
  
  <div class="mySlides fade">
    <div class="numbertext"></div>
    <img src="img/photography9.jpg" style="width:100%">
    <div class="text">Perrault Lake 2: Perrault Falls Ontario</div>
  </div> 
  
  <div class="mySlides fade">
    <div class="numbertext"></div>
    <img src="img/photography10.jpg" style="width:100%">
    <div class="text">Wasp Close Up: Thunder Bay Ontario</div>
  </div> 

  <!-- Next and previous buttons -->
  <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
  <a class="next" onclick="plusSlides(1)">&#10095;</a>
</div>
<br>

<!-- The dots/circles -->
<div style="text-align:center">
  <span class="dot" onclick="currentSlide(1)"></span>
  <span class="dot" onclick="currentSlide(2)"></span>
  <span class="dot" onclick="currentSlide(3)"></span>
  <span class="dot" onclick="currentSlide(4)"></span>
  <span class="dot" onclick="currentSlide(5)"></span>
  <span class="dot" onclick="currentSlide(6)"></span>
  <span class="dot" onclick="currentSlide(7)"></span>
  <span class="dot" onclick="currentSlide(8)"></span>
  <span class="dot" onclick="currentSlide(9)"></span>
  <span class="dot" onclick="currentSlide(10)"></span>

</div>     
</div>

<script>let slideIndex = 1;
showSlides(slideIndex);

// Next/previous controls
function plusSlides(n) {
  showSlides(slideIndex += n);
}

// Thumbnail image controls
function currentSlide(n) {
  showSlides(slideIndex = n);
}

function showSlides(n) {
  let i;
  let slides = document.getElementsByClassName("mySlides");
  let dots = document.getElementsByClassName("dot");
  if (n > slides.length) {slideIndex = 1}
  if (n < 1) {slideIndex = slides.length}
  for (i = 0; i < slides.length; i++) {
    slides[i].style.display = "none";
  }
  for (i = 0; i < dots.length; i++) {
    dots[i].className = dots[i].className.replace(" active", "");
  }
  slides[slideIndex-1].style.display = "block";
  dots[slideIndex-1].className += " active";
}
</script>
