# Javascript Library and Frameworks:

## Library
  - collection of functionality to handle strings, dates, HTML DOM elements, animations etc.
  - basically a file containing re-usable code that can be shared among multiple applications.
  - smoothens implementation details to make the work of the programmer easier.

## Framework
  - skeleton of application which calls the code to make the flow of the specific one.
  
  ![framework-vs-library](https://user-images.githubusercontent.com/26729817/29863698-12f9d9b4-8da3-11e7-8dee-c0f2e5051ccb.png)
  
## List of JS Libraries

![react](https://user-images.githubusercontent.com/26729817/29864119-5599daf2-8da4-11e7-83ef-8876b0842f90.png)


* [REACT JS](https://facebook.github.io/react/) 
  - used in applications rather than websites.
  - First library to create a virtual DOM: one way data binding which makes things simpler.

SAMPLE CODE :
 ```sh
     class HelloMessage extends React.Component {
        render() {
             return <div>Hello {this.props.name}</div>;
      }
    }
     ReactDOM.render(<HelloMessage name="Jane" />, mountNode);
 ```
  ![chartjs_logo](https://user-images.githubusercontent.com/26729817/29864424-4045011c-8da5-11e7-9442-fe6213eda00c.jpg)

* [Charts.js](http://www.chartjs.org/) 
    - an easy way to include animated, interactive graphs on your website.

 SAMPLE CODE :
 ```sh
    <canvas id="myChart" width="400" height="400"></canvas>
    <script>
     var ctx = document.getElementById("myChart").getContext('2d');
     var myChart = new Chart(ctx, {
     type: 'bar',
     data: {
        labels: ["Red", "Blue", "Yellow", "Green", "Purple", "Orange"],
        datasets: [{
            label: '# of Votes',
            data: [12, 19, 3, 5, 2, 3],
            backgroundColor: [
                     'rgba(255, 99, 132, 0.2)',
                'rgba(54, 162, 235, 0.2)',
                'rgba(255, 206, 86, 0.2)',
                'rgba(75, 192, 192, 0.2)',
                'rgba(153, 102, 255, 0.2)',
                'rgba(255, 159, 64, 0.2)'
            ],
            borderColor: [
                'rgba(255,99,132,1)',
                'rgba(54, 162, 235, 1)',
                'rgba(255, 206, 86, 1)',
                'rgba(75, 192, 192, 1)',
                'rgba(153, 102, 255, 1)',
                'rgba(255, 159, 64, 1)'
            ],
            borderWidth: 1
        }]
    },
    options: {
    scales: {
            yAxes: [{
                ticks: {
                    beginAtZero:true
                }}] }}});
     </script>
```

![momentjs](https://user-images.githubusercontent.com/26729817/29895369-76c51cd4-8e0b-11e7-992e-965406c7024b.jpeg)

  * [Moment.js](http://momentjs.com/) 
      - Parse, validate, manipulate, and display dates and times in JavaScript.
      
SAMPLE CODE: 
 ###### *FORMAT DATES*
  ```sh
    moment().format('MMMM Do YYYY, h:mm:ss a');  // August 30th 2017, 4:23:04 pm
    moment().format('dddd');                     // Wednesday
    moment().format("MMM Do YY");                // Aug 30th 17
    moment().format('YYYY [escaped] YYYY');      // 2017 escaped 2017
    moment().format();                          
```

 ###### *RELATIVE TIME*
 
 ```sh
    moment("20111031", "YYYYMMDD").fromNow(); // 6 years ago
    moment("20120620", "YYYYMMDD").fromNow(); // 5 years ago
    moment().startOf('day').fromNow();        // 17 hours ago
    moment().endOf('day').fromNow();          // in 7 hours
    moment().startOf('hour').fromNow();      
```
 ###### *CALENDAR TIME*
 ```sh
moment().subtract(10, 'days').calendar(); // 08/20/2017
moment().subtract(6, 'days').calendar();  // Last Thursday at 4:34 PM
moment().subtract(3, 'days').calendar();  // Last Sunday at 4:34 PM
moment().subtract(1, 'days').calendar();  // Yesterday at 4:34 PM
moment().calendar();                      // Today at 4:34 PM
moment().add(1, 'days').calendar();       // Tomorrow at 4:34 PM
moment().add(3, 'days').calendar();       // Saturday at 4:34 PM
moment().add(10, 'days').calendar();      // 09/09/2017   
```
     
