# Entry 4
##### 3/11/24

My tool is Math.js but another important part of my project is DOM. In order to incorporate my tool into the project, I first have to use DOM. In my HTML, I have to add button and give them ID's. Using DOM, I will then select a button, and then use math.js on that section of the code. Each recipe has its own measurements, so each recipe needs its own set of buttons for adjusting quantity of product. That button will then change the measurements of each ingredient of that recipe.

I started this with recipe one
```js
function doubleMeasurements() {
  var ingredientsList = document.getElementById("ingredients").getElementsByTagName("li");

  for (var i = 0; i < ingredientsList.length; i++) {
    var ingredient = ingredientsList[i].innerText;
    var measurement = parseFloat(ingredient.match(/\d+(\.\d+)?/));
    var unit = ingredient.match(/[a-zA-Z]+/);

    if (!isNaN(measurement)) {
      var doubledMeasurement = measurement * 2;
      ingredientsList[i].innerText = doubledMeasurement + ' ' + unit;
    }
  }
}
```
* This code is run on ever `<li>` tag within the ingredients class.
* The loop is designed to identify the measurment and unit.

* This does not yet include my tool, but it also doesn't work properly.
    * My tool is mainly just how the numbers are seen and how the are used in math.
    *Biggest issue is when the button is clicked, any whole number you chose is doubled but the ingredient name is lost.
### EDP

I am on step 5 of the engineering design process. This means I am actually starting to combine my outline of code with my actual tool and other aspects needed to make the final product.

After I write the code, I will test it. If the buttons don't properly adjust the measurments then I have to go back and improve it. I will repeat this process until all the buttons for every recipe work.

### Skills

I focused on paying attention to detail while working on this portion of my freedom project. I needed to ensure that when I created the ID in the html, that I spelt it exactly the same, with the same letters capitalized. Otherwise, when I didn't and a letter was capital in one place and not in another it didn't work.

Another skill I practiced was organization. When I work at home I have a check list of the order I code each recipe in. I start with creating the buttons, then giving them ID's, selecting them with DOM based on the ID when clicked and then coding the math. Checking off each step allows me to ensure I dont mess up a step or forget one.


[Previous](entry03.md) | [Next](entry05.md)

[Home](../README.md)