# Chart.js

This Boilerplate application comes with `Chart.js` pre-installed.

## Example

Below is a basic example of how to use Chart.js in this application

Add this to your HTML file

```html
<div class="chart-container mt-2">
    <canvas  id="MyChart" >{{ chart }}</canvas>
</div>
```

In your component you need to import Chart.js like the following:

```typescript
import Chart from 'chart.js/auto';
```

Then declare a new variable `chart`:

```typescript
public chart: any;
```

And here is an example of the definition of this variable:

```typescript
this.chart = new Chart("MyChart", {
    type: 'bar', //this denotes tha type of chart

    data: {// values on X-Axis
    labels: ['2022-05-10', '2022-05-11', '2022-05-12', '2022-05-13',
        '2022-05-14', '2022-05-15', '2022-05-16', '2022-05-17',],
    datasets: [
        {
        label: "Sales",
        data: ['467', '576', '572', '79', '92',
            '574', '573', '576'],
        backgroundColor: 'blue'
        },
        {
        label: "Profit",
        data: ['542', '542', '536', '327', '17',
            '0.00', '538', '541'],
        backgroundColor: 'limegreen'
        }
    ]
    },
    options: {
    aspectRatio: 2.5
    }

});
```