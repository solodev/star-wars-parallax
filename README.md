# star-wars-parallax
In preparation for the upcoming "Star Wars: Rogue One" film the Solodev team decided to write a Star Wars themed post on adding parallax with multiple backgrounds to your website using jQuery ScollTo by Ariel Flesler. Instead of your run of the mill stock photos, our example is filled with Tie Fighters, X-Wings, ATT Walkers, and the Death Star as backgrounds. In this article, [Solodev](https://www.solodev.com/) will teach you how to implement parallax with multiple backgrounds using gnarly Star Wars graphics.

## Tutorial

For detailed instructions, view Solodev's [A Star Wars Parallax with Multiple Backgrounds](https://www.solodev.com/blog/web-design/a-star-wars-parallax-with-multiple-backgrounds.stml) article.

## Demo

Try out a working example on [JSFiddle](https://jsfiddle.net/solodev/pa4kvfuv/).

## HTML

The parallax with multiple backgrounds contains the following basic HTML markup.

```
<div id="intro">
   <div class="story">
      <div class="float-left">
         <h2>A Star Wars Parallax: Multiple Backgrounds</h2>
         <p><p>In preparation for the upcoming "Star Wars: Rogue One" the Solodev team decided to write a Star Wars themed post on adding parallax with multiple backgrounds to your website using jQuery ScollTo by Ariel Flesler. Instead of your run of the mill stock photos, our example is filled with Tie Fighters, X-Wings, ATT Walkers, and the Death Star as backgrounds. </p> 
      </div>
   </div>
   <!--.story-->
</div>
<!--#intro-->
<div id="second">
   <div class="story">
      <div class="bg"></div>
      <div class="float-right">
         <h2>The Parallax Strikes Back</h2>
         <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean nibh erat, sagittis sit amet congue at, aliquam eu libero. Integer molestie, turpis vel ultrices facilisis, nisi mauris sollicitudin mauris, volutpat elementum enim urna eget odio.</p> 
         <p>Donec egestas aliquet facilisis. Nunc eu nunc eget neque ornare fringilla. Nam vel sodales lectus. Nulla in pellentesque eros. Donec ultricies, enim vitae varius cursus, risus mauris iaculis neque, euismod sollicitudin metus erat vitae sapien. Sed pulvinar.</p>
      </div>
   </div>
   <!--.story-->
</div>
<!--#second-->
<div id="third">
   <div class="story">
      <div class="float-left">
                <h2>The Return of Parallax</h2>
         <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean nibh erat, sagittis sit amet congue at, aliquam eu libero. Integer molestie, turpis vel ultrices facilisis, nisi mauris sollicitudin mauris, volutpat elementum enim urna eget odio.</p> 
         <p>Donec egestas aliquet facilisis. Nunc eu nunc eget neque ornare fringilla. Nam vel sodales lectus. Nulla in pellentesque eros. Donec ultricies, enim vitae varius cursus, risus mauris iaculis neque, euismod sollicitudin metus erat vitae sapien. Sed pulvinar.</p>
      </div>
   </div>
   <!--.story-->
</div>
<!--#third-->
```
## CSS

All necessary CSS is included in the file star-wars-parallax.css

## JavaScript

This tutorial utilizes the following JavaScript.

```
$(document).ready(function(){
	$('#nav').localScroll(800);
	
	//.parallax(xPosition, speedFactor, outerHeight) options:
	//xPosition - Horizontal position of the element
	//inertia - speed to move relative to vertical scroll. Example: 0.1 is one tenth the speed of scrolling, 2 is twice the speed of scrolling
	//outerHeight (true/false) - Whether or not jQuery should use it's outerHeight option to determine when a section is in the viewport
	$('#intro').parallax("50%", 0.1);
	$('#second').parallax("50%", 0.1);
	$('.bg').parallax("0%", 0.3);
	$('#third').parallax("50%", 0.3);

})
```

## External Includes

This tutorial contains the following third party resources.

```
<link href="star_wars_parallax.css" rel="stylesheet">
<link href="https://fonts.googleapis.com/css?family=Open+Sans+Condensed:300" rel="stylesheet">
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
<script src="https://www.solodev.com/assets/parallax/jquery.localscroll-1.2.7-min.js"></script>
<script src="https://www.solodev.com/assets/parallax/jquery.parallax-1.1.3.js"></script>
<script src="https://www.solodev.com/assets/parallax/jquery.scrollTo-1.4.2-min.js"></script>
```
