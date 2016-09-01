# Charts With C3.js Tutorial  
  

#### We would go through the steps for displaying data in chart form using C3.js. C3.js is a D3-based reusable chart library. D3.js is a library for manipulating and displaying data in javascript as charts. D3.js has a bit of a learning curve and requires many lines of code for displaying a chart. c3.js is a library build on top of D3.js so that we can draw charts in easily. Let's get started for some visualization!

### 1. Setup c3.js and d3.js  
  

  Create a basic html web page and include c3.js and d3.js. Download c3.js source code [here](https://github.com/c3js/c3/archive/0.4.11.zip). Extract c3.css and c3.js files located in the zip folder to your project folder. Add references to these css and js files in your html page.Importantly, include d3.js in your html script since c3.js depends on d3.js internally. 

```html
<!DOCTYPE html>
<html>
  <head>
  	<title>Purdue Ironhacks Charts with C3.js Tutorial</title>
  	<script src="https://d3js.org/d3.v4.min.js"></script>
  	<link src="/path/to/c3.css" rel="stylesheet" type="text/css">
  	<script src="/path/to/c3.js"></script>
  </head>
  <body>
    <h3>Purdue Ironhacks Charts with C3.js Tutorial</h3>    
  </body>
</html>
```

### 2. Generate Chart  
  

  C3 generates a chart by calling `generate()` with the argument object, and an element including the chart will insert into the element specified in that argument as `bindto`.

  Prepare the element to bind the chart:

  >```html<div id="chart"></div>```

  And, call `generate()` with arguments:

  >```javascript
  >var chart = c3.generate({
  >		bindto: '#chart',
  > 	data: {
  >			columns: [
  >				['data1', 30, 200, 100, 400, 150, 250],
  >				['data2', 50, 20, 10, 40, 15, 25],
  			]
  }		}
  >});
  >```

  This will show us a line chart as shown [here](https://rawgit.com/priyankjain/2016-Purdue-Ironhack-Tutorials/master/Charts-with-c3js-demo-1.html)