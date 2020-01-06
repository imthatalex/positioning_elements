# Positioning Elements Introduction

## The purpose of this repository is to simply cover the  5 main values of the Position Property: 

## 1. Static
## 2. Relative
## 3. Absolute
## 4. Fixed
## 5. Sticky

### We'll be going through each one in the order listed above, throughout this repo you will find I provided links at the end of the MD. to view the code yourself and mess around with it to better understand each type on your own, I strongly reccommend this as it will give you the best understanding. Now let's get into it.. 


# Position Type: Static

## The static position can be thought of stating you want the element to keep it's original position within the HTML structure. 

### When using static you won't be able to position elements as freely as you would when using non-static types, the purpose of static is to simply maintain it's position where it was placed within the structure, unlike FIXED which keep's the element in place regardless of the structure, we'll touch more on that down below. 

```
<style> 
    #box_static {
    border: 5px solid blue;
    width: 120px;
    height: 120px;
    margin-bottom: 10px;
    }

    #box_static div {
    background-color: green;
    height: 30px;
    width: 30px;
    position: static;
    right: 10px;
    }
</style>

<div id="box_static">
    <div></div>
</div>

```

![Image of Relative Position Type](https://i.imgur.com/05HeuK7.png)


# Position Type: Relative

## The relative type enables you to make your element non-static, meaning you can now shift the position of an element in association to it's original position. 

### In this instance let's take a look at the source code below, you can see we have the internal green square set to relative along by setting it 10px to the right. The internal square should move 10px from it's original position to the right (check image example provided below).

```
<style> 
    #box_relative {
    border: 5px solid red;
    width: 120px;
    height: 120px;
    margin-bottom: auto;
    margin-top: 100px;
    margin-left: auto;
    margin-right: auto;
    }

    #box_relative div {
    background-color: green;
    height: 30px;
    width: 30px;
    position: relative;
    right: 10px;
    }
</style>

<div id="box_relative">
    <div></div>
</div>
```

![Image of Relative Position Type](https://i.imgur.com/hhte8Sm.png)



# Position Type: Absolute

## Think of when setting an element to absolute, you're inserting that element into another world that doesn't live by your HTML structure. Absolute positions elements in association with it's parent element. 

### If you set an element that doesn't have a parent element to absolute, the parent element by default will be your html tag. The internal square this time around has a parent element called box_absolute but the element is static untli we make it ***non-static*** therfore it's going to fall under html as the parent element and position itself accoringly from the html tag. Unlike relative where it is positioned within the blue square, this time it's using the entire page to decide where to position itself, as you can see it is 10px from the right of the entire page. 

```
<style> 
    #box_absolute {
    border: 5px solid blue;
    width: 120px;
    height: 120px;
    margin-bottom: 10px;
    position: relative;
    }

    #box_absolute div {
    background-color: green;
    height: 30px;
    width: 30px;
    position: absolute;
    right: 10px;
    }
</style>

<div id="box_absolute">
    <div></div>
</div>
```

![Image of Relative Position Type](https://i.imgur.com/KZeCMQx.png)



# Position Type: Fixed 

## Remember how I stated earlier Fixed is unlike static where it doesn't keep the element structured with the rest of the page? Well just like absolute associates it's positioning with it's parent element, fixed ALWAYS associates it's positioning with the html tag. 

### When we implment the fixed position type we'll see the element be pushed to the outer part of the page similar to absolute though the main difference is the element is fixed in that exact spot, so even if the user scrolls down the page, that element will remain in the same spot. 

```
<style> 
    #box_fixed {
    border: 5px solid blue;
    width: 120px;
    height: 120px;
    }

    #box_fixed div {
    background-color: green;
    height: 30px;
    width: 30px;
    position: fixed;
    right: 10px;
    }
</style>

<div id="box_fixed">
    <div></div>
</div>


```

![Image of Relative Position Type](https://i.imgur.com/ZYX0f7n.png)



# Position Type: Sticky

## What if you wanted to have an element fixed in one spot but also be relative to the internal html structure? 

### Sticky acts as if you merged both fixed and relative together, this enables us to fix an element within our html structure and not having it be fixed outside of the page (compare the example below the exampe above for better understanding).

```
<style> 
    #box_sticky {
    border: 5px solid blue;
    width: 120px;
    height: 120px;
    }

    #box_sticky div {
    background-color: green;
    height: 30px;
    width: 30px;
    position: sticky;
    right: 10px;
    }
</style>

<div id="box_sticky">
    <div></div>
</div>

```

![Image of Relative Position Type](https://i.imgur.com/gc7zShb.png)






# Links 

## Static
https://htmlpreview.github.io/?https://github.com/imthatalex/positioning_elements/blob/7a1407c650757f079bf1216b3e3e6c8cf84e1022/relative.html


## Relative 
https://htmlpreview.github.io/?https://github.com/imthatalex/positioning_elements/blob/7a1407c650757f079bf1216b3e3e6c8cf84e1022/relative.html


## Absolute 
https://htmlpreview.github.io/?https://github.com/imthatalex/positioning_elements/blob/7a1407c650757f079bf1216b3e3e6c8cf84e1022/relative.html


## Fixed 
https://htmlpreview.github.io/?https://github.com/imthatalex/positioning_elements/blob/7a1407c650757f079bf1216b3e3e6c8cf84e1022/relative.html


## Sticky
https://htmlpreview.github.io/?https://github.com/imthatalex/positioning_elements/blob/7a1407c650757f079bf1216b3e3e6c8cf84e1022/relative.html

