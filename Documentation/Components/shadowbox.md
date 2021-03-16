### Shadow Box



#### Class

There are **2** Classes to choose from. 

1. `shadowbox-responsive_r`

2. `shadowbox-fixed_r`

   

Only width is different in the above two classes, other style is the same. The **fixed** one's width is 600px but the responsive's one's width vary according to the screen. 



#### Variable

There is **2** variable, `$blur-radius` and `$alpha`. Change those variable's value to check how does it effect.  



#### Background Color

The background color of the Shadow Box is **transparent**.  So, when you are using the above classes, also provide  a class for a suiable background color. 



#### Mixins

If you need different `$blur-radius` and `$alpha` for multiple Shadow Box, you may use mixins to do so. 



#### Code..



Change variable to change style!

```
$blur-radius: 5px;

$alpha:0.3;
```





Importing **breakpoint** sass file to use it later.

```
@import '../breakpoints';
```



**Responsive Shadow Box (Mixin) ** 



```scss
@mixin shadowbox-responsive ($blur-radius:5px, $alpha:0.2) {
    background: transparent; 
    box-shadow: 6px 6px $blur-radius rgba(0, 0, 0, $alpha);

    padding: 1.5rem;
    border-radius: 0.5rem;
    
    width:90%;

  @include mq-md {
    max-width: 700px;
  }

  @include mq-lg {
    max-width: 800px;
  }

  @include mq-xl {
    max-width: 900px;
  }

}

```



**Responsive Shadow Box (Class) ** 

```scss
.shadowbox-responsive-high_r {
  @include shadowbox-responsive(6px,0.5);
 }
```



```scss
.shadowbox-responsive-low_r {
  @include shadowbox-responsive(6px,0.3);
 }
```





**Fixed Shadow Box (Mixin)**

```scss
@mixin shadowbox-fixed ($blur-radius:5px, $alpha:0.2) {
    background: transparent; 
    box-shadow: 6px 6px $blur-radius rgba(0, 0, 0, $alpha);

    padding: 1.5rem;
    border-radius: 0.5rem;
    
    width:90%;

    max-width: 600px;
}

```



**Fixed Shadow Box (Class)**



```scss
.shadowbox-fixed-high_r {
  @include shadowbox-fixed(6px,0.5);
 }
```



```scss
.shadowbox-fixed-low_r {
  @include shadowbox-fixed(6px,0.3);
 }
```






