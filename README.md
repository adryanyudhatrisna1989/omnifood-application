# Omnifood application

### I used HTML 5, CSS 3 , JavaScript, and Jquery for this project

### Code example

```html
<header>
        <nav>
            <div class="row">
                <img src="resources/img/logo-white.png" alt="Omnifood logo" class="logo">
                <img src="resources/img/logo.png" alt="Omnifood logo" class="logo-black">
                <ul class="main-nav js--main-nav">
                    <li>
                        <a href="#features">Food delivery</a>
                    </li>
                    <li>
                        <a href="#works">How it works</a>
                    </li>
                    <li>
                        <a href="#cities">Our cities</a>
                    </li>
                    <li>
                        <a href="#plans">Sign up</a>
                    </li>
                </ul>
                <a class="mobile-nav-icon js--nav-icon">
                    <i class="ion-navicon-round"></i>
                </a>
            </div>
        </nav>
```

```jquery
/* Navigation scroll */
    $(function() {
      $('a[href*=#]:not([href=#])').click(function() {
        if (location.pathname.replace(/^\//,'') == this.pathname.replace(/^\//,'') && location.hostname == this.hostname) {
          var target = $(this.hash);
          target = target.length ? target : $('[name=' + this.hash.slice(1) +']');
          if (target.length) {
            $('html,body').animate({
              scrollTop: target.offset().top
            }, 1000);
            return false;
          }
        }
      });
    });
```
