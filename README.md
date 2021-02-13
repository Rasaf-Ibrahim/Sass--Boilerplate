> #### "It's just a note of the Sass style that I prefer and use as my default style."



### Some important Advanced topic of Sass:


#### Mixins with Arguments

If you place a set of parentheses after the name of your mixin, but before the curly braces, and fill the parentheses with a argument (or several), your mixin becomes customizable:

```
@mixin heading-shadow($colour){
    text-shadow: .55rem .55rem #15DEA5;
}

```
Think of arguments as empty variables that only live within the mixin. You set their value each time you include the mixin in your code, and that value is used within the mixin block when it is compiled to CSS.


#### Mixins with Default Arguments




