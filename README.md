# TechMart
Canvas CSS Advanced 4-1: Creating a page with what we learned in CSS Adv
This webpage is  helps you to bring all your knowledge together in one place. 
We are going to use 
  HTML:
    Semantic tags
    Relavent class names
    Structured HTML
    Featured Products Section (button Arrow Scroll)
    Hover over the product and transform
    Dialog box after submiting the form.
    Dark mode, light mode
  
Emmet:
   Nav section:   nav>div.logo>h1{TechMart}+button.hamburger#hamburger[aria-label="Toogle navigation" aria-expanded="false"]>span*3^ul#nav-menu>li*5>a^button#theme-toggle[aria-label="Toogle dark mode"]{🌙}

   Main section: 

    Product cards:
    main>header.hero>h1^section.featured-products#featured>h2+div.scroll-buttons>button#scroll-left+button#scroll-right^div.product-grid-wrapper>div.product-grid>article*10.product-card>img+div.card-content>h3+p

   New product Section:
   section.new-product#new-product>h2+div.product-highlight>div.product-image>img^div.product-info>h3+p+button.buy-btn

    Gallery section:
    section.gallery#gallery>h2+div.auto-scroll-gallery>div.gallery-track>img*8

    Contact Section:
    section.contact#contact>h2+div.contact-form>form#contactForm[action="#" method="post"]>label+input:text[placeholder="Your name"]+label+input:email[placeholder="Your email"]+label+input:text[placeholder="Subject"]+label+textarea[placeholder="Your message here"]+button:submit{Send Message}

    Dialog:
    dialog#contactDialog>h3{Thank you!}+p+button.dialog-btn#closeDialog{close}

       
  CSS:
    Responsive design 
    Hover-effects
      Hover over the image click and pop up same image
    specificity
    Flexbox
    Accessible buttons
    CSS Variables
    Media queries
    Pseudo elements
    Pseudo classes
    
  JavaScript:
    Dynamic interactions
    Event handling
    AJAX calls
    Scroll effect of gallery images
  
    

CSS properties and its usage:

scroll-behavior: smooth; is the simplest way to enable native smooth-scrolling for in-page links (anything that uses href="#section-id" or element.scrollIntoView()).

It Tells the browser to animate vertical/horizontal scrolling instead of “jumping.”

Works on any scrollable element (the whole page, or any element with overflow: auto), but setting it on html is enough for most sites.

line-height: 1.6; Because you put it on the body, that value is inherited by every element (unless an element later overrides it). So all paragraphs, list items, headings, etc., start with a line height of 1.6 × their own font size.
Example: If a paragraph inherits font-size: 16px:
/* inherited from body */
line-height = 1.6 × 16 px = 25.6 px 
So the vertical space each line occupies is ≈ 26 px, giving text room to breathe.
https://codepen.io/Htmlkodework/pen/MYYJPpw

Why the “tight” paragraph looks bigger even though the font-size is identical

Because the tight paragraph squeezes its lines closer together, the eye perceives a denser “text block.” Dense blocks feel bolder and can trick us into thinking the letters themselves are larger—even though they’re not.

More white space around the same letters makes them appear smaller; packing them tightly makes them appear larger.

Purpose of z-index:
z-index controls stacking order—which overlapping, positioned elements (those with position: relative/absolute/fixed/sticky) appear on top of which.
