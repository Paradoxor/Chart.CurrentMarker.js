# Chart.CurrentMarker.js

## Overview
This Chart.js plugin allows you to create charts similar to the one below with a marker on the right side of the chart indicating the current value.
Extension: It now allows you to add multiple "fixed" horizontal lines the chart with a marker on the left side

## Example
Have a look here for a usage example: [sample/basic.html](https://github.com/Paradoxor/Chart.CurrentMarker.js/blob/master/sample/basic.html)

This is what it can look like in action:
![Basic Example Screenshot](https://github.com/Paradoxor/Chart.CurrentMarker.js/blob/master/sample/basic.jpg)

## Configuration

To configure the current marker plugin, you can simply add new config options to your chart config.

```javascript
options: {
  currentMarker: {
    // precision of decimal in marker
    decimals: 4,

    // width of marker line
    lineWidth: 1,

    // color of marker line and marker handle
    lineColor: 'rgba(46, 153, 122, 1)',

    // dash style of marker line
    lineDash: [5, 3],

    // color of text in marker handle
    textColor: 'rgb(255, 255, 255)',

    // font size and family to use in marker handle
    font: '18px Helvetica'
  },      
  // Array of lines    
  horizontalLine: [{
    // the Y-axis position
    y: 1234,
    // color of the line and the marker
    style: 'rgba(255, 0, 0, .4)',
    // Text on the marker
    text: 'Line1'
    // line dash, textColor and font are taken from the currentMarker
  },
  {
    y: 1234 + Math.random(),
    style: 'rgba(255, 128, 0, 1)',
    text: 'Line2'
  }],


}
```
