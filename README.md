# Day 1
## Percentage VS Fixed height:
Our website are responsive if we only have HTML with no CSS. 
Giving it a fixed width & height makes it out of the responsiveness.
Give % rather than px or others to make life much easier for responsiveness.
Fix width might make things overflow where we cani use overflow hidden.
But this might cause the losing the content which can be important.
The chlid width is always the width of that % in relation with parent.
 
Its good idea to avoid the height... 
Use padding more than height for more background..like padding 5em or % or rem.

# Day 2
## The power of relative units:

em: its compounds with the parent elements and multiplies along the way
like ```child * parent * parent/body``` 
it multiples by parent if we have set there.

rem: sticks to the root elements, like 
```body {
font size: 16px
}

child 1 {
font size: 2rem;	it equals 32px
}

child 2 {
font size: 3rem;	it equalts 16 * 3 in rems
}			but in ems its 3 * 2 * 16 = 6 * 16 
```
So, thats the thing to consider.

Day 3
The power of max-width: 
it is used in big screen where the sizes stick to the size and 
doesnt go long the way... 
and makes our design more pleasent.

day 4 vh, vw, vmin,vmax
vh, vw are given while need to make it responsive on all devices 
vmin,vmax are used where which one is highest is used.

Title can be used as per vw to make it responsive.
It doesn't work much with the paras but vh might be useful.

Vh is used popular ... for titles it might be useful.
Need to use the media queries for the both the sizez.
where one time it can get really big next time in really short screen.

Day 5 are challenge.


Day 6: 
Dont use em's for fornt sizes.
Because of the compound effect on the em's as they look towards the parents and keep increasing like 1.25 * 1.25 * 1.25 .... ouch so big

works for parents and sibligns where siblings takes its and * parents.


:root{
font-size: 10px;
}

use rem instead or em's as it reference to that root....

but use em to padding as at that time its referencing to font-size rather than its parent where there is no compound effect.

can use it for margin bottom or other cases.\

    width: 600px; max-width: 100%;
    width: 100%; max-width: 600px;

This might be a useful way to think about it: if the element would render wider than what max-width says it can be, max-width wins.

Day 7 challenge #3

Day 8 - Flexbox
Flex-container 
flex-items = smallest possible size. - width 100% or height - 100%
spacing in the flex-item = 

gap: 100px;


we can use also: 

Combinators: select the adjecent siblings

col + col {
	margin-left: 10px;
}

then the flexbox challenge.


Day 9 : 

reducing the amount of HTML container 

container and row in same div's .. concept is not to mix the to classes.


flex stretch the elements to be of equal heights..

align-self: flex start or the use of the divs elements for keeping the items aligns 


jusitfy content : space-between ... makes the use of space rather than the margins or other uses.

flex items when less like 30% for each item it can be related and adjusts into those sizes but when 100% it will make it equal for both the element.


Day 11 : 
img {
max-width: 100%
}

the concept of flex-grow and flex-shrink 

flex-grow allows the element to grow as much space avaialable where as flex shrink allows to shrink it to as much as it needs when the screen shrinks...

Day 13/14 :
More on min(), max() and clamp()


Day 15: 
order of media is imp and then there are lot of media for speech print and lot more ..

Having less breakpoint is good plus the more the harder to maintain.

Day 17: 
the importance of meta tag and initial scale is 1.0 



