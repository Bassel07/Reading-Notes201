# Docs for the HTML canvas Element & Chart.js

Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them 
into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.

A great way to get started with charts is with Chart.js, a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page.
It’s a well documented plugin that makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy.

To see how to use chart.js we’re going to create a set of 3 graphs;
one will show the number of buyers a fictional product has over the course of 6 months, this will be a line chart;
the second will show which countries the customers come from, this will be the pie chart;
finally we’ll use a bar chart to show profit over the period.

# www.chartjs.org

![image](https://user-images.githubusercontent.com/85109819/124451254-0e23c900-dd3a-11eb-8454-e6cb6c3ec269.png)



![image](https://user-images.githubusercontent.com/85109819/124456657-d1f36700-dd3f-11eb-9bc9-4e48b560089b.png)


![image](https://user-images.githubusercontent.com/85109819/124456916-1c74e380-dd40-11eb-84d0-2a898894c1e3.png)

https://github.com/chartjs/Chart.js


# Basic usage of canvas

![image](https://user-images.githubusercontent.com/85109819/124458261-9bb6e700-dd41-11eb-9d84-c652c7ac22cd.png)


# Drawing shapes with canvas


![image](https://user-images.githubusercontent.com/85109819/124458556-f81a0680-dd41-11eb-8867-0214dfe3a8cf.png)


# Applying styles and colors

![image](https://user-images.githubusercontent.com/85109819/124458911-6ced4080-dd42-11eb-8520-967bdc98c855.png)

![image](https://user-images.githubusercontent.com/85109819/124458998-88f0e200-dd42-11eb-80fa-478741c56437.png)

# Drawing text

![image](https://user-images.githubusercontent.com/85109819/124459270-d79e7c00-dd42-11eb-8a24-339cefed5c14.png)

![image](https://user-images.githubusercontent.com/85109819/124459332-e5ec9800-dd42-11eb-8eba-0ddcc69d5071.png)

![image](https://user-images.githubusercontent.com/85109819/124459452-fd2b8580-dd42-11eb-81e4-af1bcf0bf026.png)

Setting up
The first thing we need to do is download Chart.js. Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in.
Then create a new html page and import the script:

![image](https://user-images.githubusercontent.com/85109819/124468666-3ddccc00-dd4e-11eb-9578-08138462a889.png)


# Drawing a line chart 

To draw a line chart, the first thing we need to do is create a canvas element in our HTML in which Chart.
js can draw our chart. So add this to the body of our HTML page:

![image](https://user-images.githubusercontent.com/85109819/124468742-5baa3100-dd4e-11eb-9f3b-f2541aa700e3.png)

Next, we need to write a script that will retrieve the context of the canvas, so add this to the foot of your body element:

![image](https://user-images.githubusercontent.com/85109819/124468856-7da3b380-dd4e-11eb-88a8-c4c2fda162e9.png)

(We can actually pass some options to the chart via the Line method, but we’re going to stick to the data for now to keep it simple.)

# Drawing a pie chart

Our line chart is complete, so let’s move on to our pie chart. First, we need the canvas element:

![image](https://user-images.githubusercontent.com/85109819/124468999-a5931700-dd4e-11eb-8d8a-d03ec621a4b7.png)

Next, we need to get the context and to instantiate the chart:

![image](https://user-images.githubusercontent.com/85109819/124469128-d3785b80-dd4e-11eb-98ed-2f54c8092198.png)


https://www.webdesignerdepot.com/cdn-origin/uploads7/easily-create-stunning-animated-charts-with-chart-js/chartjs-demo.html

![image](https://user-images.githubusercontent.com/85109819/124469375-23efb900-dd4f-11eb-8075-05dd4cbf9544.png)

![image](https://user-images.githubusercontent.com/85109819/124469431-3833b600-dd4f-11eb-93cb-e37ae229af8f.png)
















