> #### "It's just a note of the Sass style that I prefer and use as my default style."



### Some important Advanced topic of Sass:


#### Mixins:


##### Mixins with Arguments

If you place a set of parentheses after the name of your mixin, but before the curly braces, and fill the parentheses with a argument (or several), your mixin becomes customizable:

```

@mixin heading-shadow($colour){
    text-shadow: .55rem .55rem #15DEA5;
}

```
Think of arguments as empty variables that only live within the mixin. You set their value each time you include the mixin in your code, and that value is used within the mixin block when it is compiled to CSS.


```

 .heading{
    @include heading-shadow(#ffffff);
    }
 }
 
 ```

And when you check out the compiled CSS code, the heading header has a white shadow!


```
.heading{
  text-shadow: 0.55rem 0.55rem #ffffff;
}

```


##### Mixins with Default Arguments

Rather than having to enter a color value each time you use your **heading-shadow** mixin, you can set the default value for the argument. Then, if you decide not to customize the shadow's color, it will use the default instead. Do this by defining its value just like a normally declared variable:

```

@mixin heading-shadow($colour: #000000){
    text-shadow: .55rem .55rem $colour;
}

```

Now, if you omit the argument and don’t set a color value when you include it, Sass will assume that you want the shadow to be the default color, **#000000**.








