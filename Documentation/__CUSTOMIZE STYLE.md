## How to customize the Sass Style by using Variable



Create a  **.scss** file and  change any variable's property there.  Then import your .scss file  into **custom.scss** file which you will get inside the **Scss** folder. That's it!



### What's happenning behind the scene

Let's understand  behind the scene by focusing on **shadowbox.scss** file (This file is in the component folder).



In the **shadowbox.scss** file, all the varibales is declared at first. After defining the variable, **custom.scss** file is imported.  Now suppose, someone has changed shadowbox.scss's  variables by creating there own .scss file and importing their file in custom.scss file. By doing this, their file is  also getting imported in the shadow.scss file automatically and effecting the style.



All other files are created exactly in the same way as **shadowbox.scss**. So, the system will work in the same way too.