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

# Day 3
## The power of max-width:
it is used in big screen where the sizes stick to the size and doesn't go long the way...and makes our design more pleasent.

# Day 4 
About vh, vw, vmin,vmax:
vh, vw are given while need to make it responsive on all devices 
vmin,vmax are used in which the highest value either height or width is used.

Title can be used as per vw to make it responsive.
It doesn't work much with the paragraphs but vh might be useful in terms of smaller devices.

Vh is used more often ... for titles as it might be useful.
Need to use the media queries for the both the sizes where one time it can get really big, next time in really short screen.

# Day 5 

Completed the Challenge 2.

# Day 6
Dont use em's for font sizes.
Because of the ```compound effect``` on the em's as they look towards the parents and keep increasing like ```1.25 * 1.25 * 1.25``` .... ouch so big

Works for parents and sibligns where siblings takes its and * parents.


```
:root{
font-size: 10px;
}
```

Use rem instead or em's as it reference to that root but use em to padding as at that time its referencing to font-size rather than its parent where there is no compound effect.

Can use it for margin bottom or other cases.

```
width: 600px; max-width: 100%;
width: 100%; max-width: 600px;
```

This might be a useful way to think about it: if the element would render wider than what max-width says it can be, max-width wins.

# Day 7

Completed the challenge #3

# Day 8 - Flexbox
About Flex-container 
flex-items = smallest possible size. either use ```width 100% or height - 100%```

How to do spacing in the flex-item = 

```
gap: 100px;
```

Or, we can use also use: 

Combinators: select the adjecent siblings

```
col + col {
	margin-left: 10px;
}
```

Then the flexbox challenge #1.

# Day 9

Reducing the amount of HTML container 

container and row in same div's .. concept is not to mix the two classes.

flex stretch the elements to be of equal heights..

```align-self: flex start or the use of the divs elements for keeping the items aligns```

```jusitfy content : space-between ... makes the use of space rather than the margins or other uses.```

FLEX ITEMS when less like 30% for each item it can be related and adjusts into those specific sizes 
but when 100% it will make it equal for both the element.


# Day 11 : 

## How to make image responsive:

```
img {
max-width: 100%
}
```
The concept of flex-grow and flex-shrink: 

flex-grow allows the element to grow as much space avaialable where as flex shrink allows to shrink it to as much as it needs when the screen shrinks...

# Day 13/14
More on min(), max() and clamp() (Future Research).


# Day 15

How to use the media queries plus the Order of media query's are important and then there are lot of media queries avaialble like for speech print and lot more (Future Research).

Having less breakpoint is good plus the more the harder to maintain.

# Day 17

The importance of meta tag and initial scale is 1.0 

``` <meta name="viewport" content="width=device-width, initial-scale=1.0">```

# Day 18/19/20

Completed other Flex's challenges.

