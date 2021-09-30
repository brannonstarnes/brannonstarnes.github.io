# Reading 12

## A Handy Guide to Chart.js

1. Download [Chart.js](https://cdnjs.com/libraries/Chart.js). 
2. Import the script ```<script src='Chart.min.js'></script>``` into your HTML. This should go in ```<head>```
3. Create a canvas element in HTML where the chart will be drawn  ```<canvas id='myChart' width='600' heigh="400"></canvas>``` 
4. Add ```<script>``` element to foot of ```<body>```. Ex:
      ```<script src="path/to/chartjs/dist/chart.js"></script>
         <script>
           var myChart = new Chart(ctx, {...});
         </script>
         

Another way to accomplish this is using the following script:
 ```<script>```
``` var buyers = document.getElementById('buyers').getContext('2d');```
``` new Chart(buyers).Line(buyerData);```
``` </script>```

This will produce a line chart, whereas below will produce a pie chart  :

```var countries= document.getElementById("countries").getContext("2d");```
```new Chart(countries).Pie(pieData, pieOptions);```
 
 The full documentation and each of the types of charts can be found [here](https://www.chartjs.org/docs/latest/getting-started/integration.html).
