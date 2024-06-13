# Entry 5
##### 05/03/24

### Content

To learn my tool I have tried methods of incorporating it into my freedom project. Since its main purpose was only to make the numbers look better, all it required was for me to use `math.fraction()` and put the actual math I needed done within the parenthesis. 
``` js
var originalMeasurement = measurements[0];
var originalFraction = math.fraction(originalMeasurement);
var doubledFraction = math.fraction(originalFraction.n * 2, originalFraction.d);     
```
In this case, each measurement was in an array. First the origionalFraction variable ensure it eas a fraction. Then, the doubleFraction variable multiplied the numerator of the fraction (origionalFraction.n) by 2 to double it. For the button that is used to half the recipe, it uses the same code but instead of doubleing the numerator it double the denominator.  

I used the [math.js](https://mathjs.org/docs/index.html) libraries to learn how to differentiate the numerator and the denominator in code.

### Engineering Design Process

I have now completed step 6 of the EDP which is to Test my project. I have created my MVP or minimun valued product. While it does what I want it to, there are always improvments to be made. Such as formatting. Making it more appealing. Or extending it and adding more recipes as right now it only has 1. This would all be considered step 7 of the EDP which is to Improve. After that all thats left in this process is to share my project with my community. 

### Skills

I frequently used the skill of debugging during the creation process. I spent a lot of time debugging my functions to ensure no key information was lost when the function was ran. At first when the button was pressed to double the recipe, it would only display the measurement. For example, the origional would say "1/2 cup unsalted butter", and then after the button was pressed it would only say "1" with no unit of measurement or ingredient name. For the sake of a recipe, this was not very practical. What I learnt was that I would need code in my function that would identify the unit and ingredient of each list item and reuse it when rewriting that line. 

[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
