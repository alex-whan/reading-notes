# Reading 12: Docs for the HTML \<canvas\> Element & Chart.js

### Chart.js

* **Chart.js** is a JavaScript **plugin** that utilizes the canvas elements of HTML5 to draw a graph/chart on the page

* Options include:
  - Bar charts
  - Line charts
  - Pie charts

#### Creating a Chart on Chart.js

* Charts can be made through Chart.js by including the appropriate script and a single `<canvas>` node to render it

* First step of drawing a chart is the create a `<canvas>` element in the HTML

* Example:
`<canvas id="buyers" width="600" height="400"></canvas>`

* Then, write a script to retrieve that canvas' context at the end of the body element:

    <script>
      var buyers = document.getElementById('buyers').getContext('2d');
      new Chart(buyers).Line(buyerData);
    </script>

* Inside the script, we also need to create our data (can be an object with labels for the chart and the datasets themselves):

      <script>
        var buyerData = {
          labels : ["January", "February", "March", "April", "May", "June"],
          datasets : [
            {
              fillColor : "rgba(172,194,132,0.4)",
              strokeColor : "#ACC26D",
              pointColor : "#fff"
              pointStrokeColor : "#9DB86D",
              data " [203,156,99,251,305,247]
            }
          ]
        }
      </script>

Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)