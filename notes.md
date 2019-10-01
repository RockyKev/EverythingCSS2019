# Random Notes

## Things I personally forget: 
* text-decoration == about lines (overline, line-through, underline)
* Creating a menu burger = Unicode directly ```&#9776```;
* padding = inside; margin = outside. 
	
### CSS Patterns: 
* Standard website (navbar, sidebar, content, footer)
	
### Borders: 
* Border-styles: dotted, dashed, solid, double. (3D - groove, inset, outset)
* box-shadow: 5px 5px 5px 5px red [hori,vert,blur,spread,color]
** ---inset to invert it. 
		
### Transform: 
* transform: skew(10deg, 10deg) rotate(-10deg) scale(2, 2), translate(20px, 10px)
* translate is like position from origin, but efficient.
* transition - use this with a psuedoclass. 
```
.img {
    transition: transform .2s ease-in;
    }
    
.img:hover {
    transform: skew(50deg, 50deg);
}
```

### Animate
* define THEN call.
* DEFINE with @keyframes [name]
* OPTION 1: with from { } and to { }
* OPTION 2: with percentages 0% { } 10% { } 50% { } 100 { }

* CALL with animation-name
* animation-name, animation-duration, animation-timing-function, animation-iteration-count;

animation-fill-mode: forwards;   
//ends the animation at the last frame

animation-fill-mode: backwards; 
//starts the animation on the first frame.

animation-fill-mode: both; 

https://static.md/ed4bcad4d4295c2844ba1b424a7cb55c.png



###


## Links
Borders: 
	* drawing eggs: https://www.htmldog.com/guides/css/advanced/roundedcorners/

Transforming: 
	* Skewing https://www.htmldog.com/guides/css/advanced/transformations/

Positioning: 

Colors: 
	Color names: https://www.rapidtables.com/web/css/css-color.html
	Gradients: https://www.htmldog.com/guides/css/advanced/gradients/
	Filters: https://developer.mozilla.org/en-US/docs/Web/CSS/filter

Flexbox: 
	CSS zombies -
	https://codepip.com/games/flexbox-froggy/

Grid: 
	https://learncssgrid.com/
	https://cssgridgarden.com/

Animation: 
	keyframes: https://thoughtbot.com/blog/css-animation-for-beginners
	basics: https://css-tricks.com/almanac/properties/a/animation/
	direct code: https://github.com/all-animation/all-animation/blob/master/assets/css/all-animation.css

Drawing graphics: 
	CSS Shapes: https://css-tricks.com/the-shapes-of-css/
	Shape Design: https://css-tricks.com/working-with-shapes-in-web-design/
	

## Recipes
Positioning: 

Colors: 

Flexbox: 

Grid: 

### Animation: 
```
<style> 
  @keyframes slide {
    from {transform: translateX(0);}
    to {transform: translateX(900px);}
  }
  
  #animate:hover {
    animation-name: slide;
    animation-duration: 2s;
    animation-timing-function: ease-in;
    animation-iteration-count:  
  }
  
</style>
```



### Transform-transition: 
```
<style>
  img {
    transform: rotateY(45 deg); 
    transition: transform .2s ease-in, border .2s .5s ease-in;
    border: 2px dotted black;
  }
  
  img:hover {
    border: 10px solid black;
    transform: scale(2);
  }
</style>

  <img src="https://www.placecage.com/200/200">

```
Explain: 
> transition: transform .5s ease-in; 
Transition: css element, time to complete, curve

> border .2s .5s ease-out;
Transition: css element, time delay, time to complete, curve




Drawing graphics: 
	

SHAPES: 
```
#egg {
    background: #fff;
    width: 100px;
    height: 150px;
    border-radius: 50px/100px;
    border-bottom-left-radius: 50px;
    border-bottom-right-radius: 50px;
  }
```

```
  /* menu */
  ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    overflow: hidden;
    background: orange;
  }
  
  li {
    display: block;
    width: 60px;
    padding: 16px 16px;
    float: left;
  }
  
  li:nth-of-type(5) {
    float: right;
  }
```  


