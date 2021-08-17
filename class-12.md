# Element & Chart.JS

## JavaScript Charts

- Using charts for displaying data allows the viewer to see a clear story of the data you are showing. To do this in **JavaScript** it is necessary to download **Chart.js** plugin.

- Some typical charts used are line, pie, and a bar chart.

## Line Chart

- First it requires us to create a **Canvas** element:
    `<canvas id=" " width="800" height="400"></canvas>`
- This provides us with the area to draw our chart.

    `<script>`
        `var  = document.getElementById('').getContext('2d');`
        `new Chart().Line();`
    `</script>`
- This code allows us to grab the element and pass in our new line graph

### Data

- To input data we need to create a variable that contains the data:
    `let data= {`
        `labels:[     ],`
        `datastes :[ {`
            `fillcolor:`
           `strokcolor:`
           `pointcolor:`
           `pointstorkecolor:`
           `data:[]`
       `}]`
  `}`
- The code with **Color** following will be for line design while the actual **Data** will be stored in the array data.

## Pie Chart

- Similar to the line graph we need to create a canvas to work on then grab that canvas to pass in our graph:

    `var = document.getElementById().getContext("2d");`
    `new Chart().Pie(, );`
- The biggest difference between the line graph data and the pie graph is we will be generating format for each data value separately:

    `var pie = [`
        `{`
           `value: 45,`
           `color: rgb`
        `},`
    `]`
- After inputing the data you can then add options for the pie graph such as animations.

## Bar Chart

- As shown above the first step is to create a canvas to work on and then grab the element:
    `var  = document.getElementById().getContext("2d");`
    `new Chart().Bar();`
- Then we add the data which is very similar to how we added the line chart data:
    `var name = {`
	`labels : [],`
	`datasets : [`
	`{`
	`fillColor : rgb,`
	`strokeColor : rgb,`
	`data : []`
	`},`

- Using these charts is a great way to provide a proper story for your data and this plugin is very flexible and will allow you to add animation and flare to your presentation

# Useful Links

- [EASILY CREATE STUNNING ANIMATED CHARTS WITH CHART.JS](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)