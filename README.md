# basics

CSS
----
* Change image at reponsive

img src="images/banner01-mobile.webp" srcset="images/banner01-mobile.webp 480w, images/banner01.webp 1400w" alt="..." style="width: 100%;"

* bootstrap remove outline
textarea:focus,
input[type="text"]:focus,
textarea[type="text"]:focus,
input[type="password"]:focus,
input[type="datetime"]:focus,
input[type="datetime-local"]:focus,
input[type="date"]:focus,
input[type="month"]:focus,
input[type="time"]:focus,
input[type="week"]:focus,
input[type="number"]:focus,
input[type="email"]:focus,
input[type="url"]:focus,
input[type="search"]:focus,
input[type="tel"]:focus,
input[type="color"]:focus,
.uneditable-input:focus,
.form-control:focus {
    border-color: none;
    box-shadow: none;
    outline: none;
}


jQuery
-----------
* prefixfree.js

* Animate on scroll
https://michalsnik.github.io/aos/
https://www.jqueryscript.net/demo/Animate-Elements-In-Sequence-jQuery-CSS3-Animation-Queue/

* Slide animation on scroll
https://www.jqueryscript.net/animation/jQuery-Plugin-To-Create-Elements-Fly-in-Effects-On-Scroll.html

* counter up number effect
https://github.com/ciromattia/jquery.counterup

* custom scrollbar
http://manos.malihu.gr/jquery-custom-content-scroller/

* lazy load images, videos, etc :
lozad js

* dynamically add edit delete list / table
https://www.jqueryscript.net/form/Dynamic-Form-Creation-Deletion.html


* JavaScript
    <!-- Animate navbar on scrolldown -->
    <script>
      let nav = document.getElementById("nav2"); // Identify target
      let logo = document.getElementById("logo");
      let carouselImg = document.querySelectorAll(".carousel-img");

      window.addEventListener("scroll", function(event) {
        // To listen for event
        event.preventDefault();

        if (window.scrollY <= 29) {
          // Just an example
          nav.style.background = "transparent"; // or default color
          nav.style.padding = "50px 0 0 0";
          logo.style.width = "150px";
          for (let i = 0; i < carouselImg.length; i++) {
            carouselImg[i].style.filter = "brightness(40%)";
          }
        } else {
          nav.style.background =
            "linear-gradient(to right,rgba(72, 0, 72, 0.9), rgba(192, 72, 72, 0.9))";
          nav.style.padding = "5px 0";
          logo.style.width = "125px";

          for (let i = 0; i < carouselImg.length; i++) {
            carouselImg[i].style.filter = "brightness(100%)";
          }
        }
      });
    </script>
