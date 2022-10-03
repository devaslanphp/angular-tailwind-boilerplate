# Angular Tailwind Boilerplate

This is a project based on Angular and integrate Tailwind with a basic setup to let you quickly start your new application based on this technologies.

![Webpack](https://img.shields.io/badge/webpack-%238DD6F9.svg?style=for-the-badge&logo=webpack&logoColor=black)
![NPM](https://img.shields.io/badge/NPM-%23000000.svg?style=for-the-badge&logo=npm&logoColor=white)
![Yarn](https://img.shields.io/badge/yarn-%232C8EBB.svg?style=for-the-badge&logo=yarn&logoColor=white)
![Angular](https://img.shields.io/badge/angular-%23DD0031.svg?style=for-the-badge&logo=angular&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)
![SASS](https://img.shields.io/badge/SASS-hotpink.svg?style=for-the-badge&logo=SASS&logoColor=white)

## What's inside?
- [x] [Angular](https://angular.io/)
- [x] [TailwindCSS](https://tailwindcss.com/)
- [x] [Fontawesome](https://fontawesome.com/)
- [x] [Chart.js](https://chartjs.org/)

## Prerequisites

This project is created using `@angular/cli` so we recommend you to install this tool with the command:

```bash
npm i -g @angular/cli
```

## Installation

1. Clone this repository into your development environment
2. Install dependencies `npm install` (or `yarn install`)
3. Serve the application `ng serve`

## Chart.js example

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
    type: 'bar',

    data: {
        labels: [
            '2022-05-10', '2022-05-11', '2022-05-12', '2022-05-13',
            '2022-05-14', '2022-05-15', '2022-05-16', '2022-05-17',
        ],
        datasets: [
            {
                label: "Sales",
                data: [
                    '467', '576', '572', '79', '92',
                    '574', '573', '576'
                ],
                backgroundColor: 'blue'
            },
            {
                label: "Profit",
                data: [
                    '542', '542', '536', '327', '17',
                    '0.00', '538', '541'
                ],
                backgroundColor: 'limegreen'
            }
        ]
    },
    options: {
        aspectRatio: 2.5
    }
});
```
---

**Enjoy Coding!**
