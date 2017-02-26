---
layout: project
project: CSS Zen Garden
project-brief: Power of CSS
permalink: /work/csszen/
id: csszen
live: http://casiemattrisch.com/CSS-Zen-Garden/
github: https://github.com/cczapski/CSS-Zen-Garden
preview: /images/work/css_zen/home_laptop_css_zen.png
technologies: CSS and Sass
short: This project is an exploration of working solely with CSS to style a webpage. The design is inspired by the De Stijl movement of the early 1900's. You can view the original CSS Zen Garden website <a href="http://www.csszengarden.com/">here</a>.
---
##### Research
Initially unfamiliar with the De Stijl art movement, I began the project with research. I discovered the main concepts of the style center on simplicity with a focus on the very basics in both color and shape.

<p class="de-stijl-piece">
    <img alt="Example of De Stijl Art" src="/images/work/css_zen/de_stijl_piece.png">  
</p>

The artists and architects that created the movement believed in the use of only primary colors and black and white. Lines are straight, horizontal and vertical with only squares and rectangles for shapes. Asymmetrical arrangement is also a key aspect of the style. 

##### The Style (or in Dutch, De Stijl)

I wanted my CSS Zen Garden to fully encompass all aspects of De Stijl and initially I thought this would be fairly easy to achieve based on the simplicity of colors and shapes.

<p class="type-sample">
    <img alt="Example of Play Type" src="/images/work/css_zen/type_sample.jpg">  
</p>

The type, Play by Google Fonts, matches the basic geometric structure of the style.

The square and rectangular shapes were fairly easy to create with CSS borders, and the blocks of color are inserted using pseudo classes with before and after properties.

For an added touch, I experimented with CSS animations to give the initial landing page a full, non-text example of De Stijl by covering the blocks of text with primary colors. CSS animations allowed me to then gradually fade out the colors to reveal the text on the page.

##### Biggest Challenge
A goal I set for the project was to avoid using any images to replicate the De Stijl movement. Initially, I was unable to figure out how to add horizontal and vertical lines in the background of the basic shapes. After much experimentation, I discovered a way to create repeating horizontal lines with linear gradients.

To improve the project from its current state, I will be exploring methods to add in repeating vertical lines as well, which I think will enhance the overall design to more closely emulate De Stijl.

<div class="devices">
    <p class="small small-de-stijl">
        <img alt="Small Device CSS Zen Garden" src="/images/work/css_zen/de_stijl_small.png">
    </p>

    <p class="medium">
        <img alt="Medium Device CSS Zen Garden" src="/images/work/css_zen/de_stijl_medium.png">
    </p>
</div>

<a class="credit" href='http://www.freepik.com/free-vector/screens-collection-free-vector_713789.htm'>Devices designed by Freepik</a>