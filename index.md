---
layout: layout.html
title: Reese Pattison Portfolio
eleventyNavigation:
     key: Home

---
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
<div class="TitleDiv">

# {{ title }} 


### Click the dots to see some of my works!

</div>
<!-- Slideshow container -->
<div class="slideshow-container">

  <!-- Full-width images with number and caption text -->
  <div class="mySlides fade">
    <div class="numbertext"></div>
    <img src="img/photography3.jpg" style="width:100%">
    <div class="text">Red Lake Ontario Lake side.</div>
  </div>

  <div class="mySlides fade">
    <div class="numbertext"></div>
    <iframe class="Video1" width="2140" height="1200" src="https://www.youtube.com/embed/VZV3J6Jus_8?controls=0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    <div class="text">Demo Logo Animation (Cinema 4D & Adobe After Effects)</div>
  </div>

  
  <div class="mySlides fade">
    <div class="numbertext"></div>
    <img src="img/photography5.jpg" style="width:100%">
    <div class="text">Close Up Of Flowers: Red Lake Ontario</div>
  </div>
  <div class="mySlides fade">
    <div class="numbertext"></div>
    <img src="img/3D_3.jpg" style="width:100%">
    <div class="text">Beach Fire (made & Rendered In Maya)</div>
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
</div>     
</div>
