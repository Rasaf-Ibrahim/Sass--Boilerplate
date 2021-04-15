 ### Font Family



####  Google Font

```scss
@import url('https://fonts.googleapis.com/css2?family=Indie+Flower&family=Lobster+Two family=Open+Sans&family=Roboto+Mono&display=swap');
```



**Imported font-family in the above link:**

`font-family: 'Open Sans', sans-serif;` 

`font-family: 'Roboto Mono', monospace;` 

`font-family: 'Lobster Two', cursive;` 

`font-family: 'Indie Flower', cursive;` 





By default, the font family will be **Open sans**. But you can choose **font-monospace** or **font-cursive** to class to change the style.



```scss
html{
  font-family: 'Open Sans', sans-serif; 
}


.font-monospace {
  font-family: 'Roboto Mono', monospace;
}


.font-cursive {
  font-family: 'Lobster Two', cursive;
}

```









### Font Size



```css
@import 'breakpoints';
```



**Mobile Screen**

```css

.font-6_r {
  font-size: 2.5rem; //40px
}

.font-5_r {
  font-size: 1.75rem; //28px
}

.font-4_r {
 font-size: 1.3125rem; //21px
}

.font-3_r {
  font-size: 1.125rem; //18px
}

.font-2_r {
  font-size: 0.9375rem; //15px
}


.font-1_r {
  font-size: 0.75rem; //12px
}
```

 



**Tablet and Laptop**



```css
@include mq-md{

.font-6_r {
  font-size: 3rem; //48px
}

.font-5_r {
  font-size: 2rem; //32px
}

.font-4_r {
 font-size: 1.5rem; //24px
}

.font-3_r {
  font-size: 1.25rem; //20px
}

.font-2_r {
  font-size: 1rem; //16px
}


.font-1_r {
  font-size: 0.8125; //13px
}

}
```



**Dekstop and Extra Large Screen**



```css
@include mq-xl {

 .font-6_r {
    font-size: 3.5rem; //56px
  }

 .font-5_r {
    font-size: 2.25rem; //36px
  }

 .font-4_r {
   font-size: 1.75rem; //28px
 }


 .font-3_r {
  font-size: 1.375rem; //22px
}

  .font-2_r {
    font-size: 1.125rem; //18px
  }


  .font-1_r {
    font-size: 0.875; //14px
  }

}
```







