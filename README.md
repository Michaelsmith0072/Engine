# Engine
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <title>Nutrition Label</title>
    <link href="https://fonts.googleapis.com/css?family=Open+Sans:400,700,800" rel="stylesheet">
    <link href="./styles.css" rel="stylesheet">
  </head>
  <body>
    <div class="label">
      <header>
        <h1 class="bold">Nutrition Facts</h1>
        <div class="divider"></div>
        <p>8 servings per container</p>
        <p class="bold">Serving size <span class="right">2/3 cup (55g)</span></p>
      </header>
      <div class="divider lg"></div>
      <div class="calories-info">
        <p class="bold sm-text">Amount per serving</p>
        <h1>Calories <span class="right">230</span></h1>
      </div>
      <div class="divider md"></div>
      <div class="daily-value sm-text">
        <p class="right bold no-divider">% Daily Value *</p>
        <div class="divider"></div>
        <p><span class="bold">Total Fat</span> 8g<span class="bold right">10%</span></p>
        <p class="indent no-divider">Saturated Fat 1g <span class="bold right">5%</span></p>
        <div class="divider"></div>
        <p class="indent no-divider"><i>Trans</i> Fat 0g</p>
        <div class="divider"></div>
        <p><span class="bold">Cholesterol</span> 0mg <span class="right bold">0%</span></p>
        <p><span class="bold">Sodium</span> 160mg <span class="right bold">7%</span></p>
        <p><span class="bold">Total Carbohydrate</span> 37g <span class="right bold">13%</span></p>
        <p class="indent no-divider">Dietary Fiber 4g</p>
        <div class="divider"></div>
        <p class="indent no-divider">Total Sugars 12g</p>
        <div class="divider dbl-indent"></div>
        <p class="no-divider dbl-indent">Includes 10g Added Sugars <span class="bold right">20%</span></p>
         <div class="divider"></div>
      </div>
    </div>
  </body>
</html>


CSS
* {
  box-sizing: border-box;
}

html {
  font-size: 16px;
}

body {
  font-family: 'Open Sans', sans-serif;
}

.label {
  border: 2px solid black;
  width: 270px;
  margin: 20px auto;
  padding: 0 7px;
}

header h1 {
  text-align: center;
  margin: -4px 0;
  letter-spacing: 0.15px
}

p {
  margin: 0;
}

.divider {
  border-bottom: 1px solid #888989;
  margin: 2px 0;
  clear: right;
}

.bold {
  font-weight: 800;
}

.right {
  float: right;
}

.lg {
  height: 10px;
}

.lg, .md {
  background-color: black;
  border: 0;
}

.md {
  height: 5px;
}

.sm-text {
  font-size: 0.85rem;
}

.calories-info h1 {
  margin: -5px -2px;
  overflow: hidden;
}

.calories-info span {
  font-size: 1.2em;
  margin-top: -7px;
}

.indent {
  margin-left: 1em;
}

.dbl-indent {
  margin-left: 2em;
}

.daily-value p:not(.no-divider) {
  border-bottom: 1px solid #888989;
}
