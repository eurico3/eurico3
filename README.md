<!--
### Hi there 👋


<!--
**eurico3/eurico3** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<a href="https://www.linkedin.com/in/euricopaes/">
  <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)" alt='Twitter'>
</a>

<p>
$$ {J(\theta) =\frac{1}{2m} [\sum^m_{i=1}(h_\theta(x^{(i)}) - y^{(i)})2 + \lambda\sum^n_{j=1}\theta^2_j} $$
</p>
-->
<a href="https://github.com/eurico3/eurico3">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=eurico3&&layout=compact&bg_color=00000000&text_color=#ffffff" />
</a>
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Flask & Apexcharts</title>

    <!-- Bootstrap -->
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">
    
    <!-- Bootstrap Icons-->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
    
    <!-- Font Awesome CSS -->
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" rel="stylesheet">

    <!-- Apex Charts -->
    <script src="https://cdn.jsdelivr.net/npm/apexcharts"></script>

    <style>

      #gitlogo {
        padding: 20px;
      }
    </style>




    <body>
        <nav class="navbar navbar-dark bg-dark fixed-top">
      
            <div class="container-fluid">
    
           
              
              <button class="navbar-toggler" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasDarkNavbar" aria-controls="offcanvasDarkNavbar" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
              </button>
              <a class="navbar-brand" href="#">

                Flask & Apexcharts</a>
              <!-- <div class="offcanvas offcanvas-end text-bg-dark" tabindex="-1" id="offcanvasDarkNavbar" aria-labelledby="offcanvasDarkNavbarLabel"> -->
              <div class="offcanvas offcanvas-start text-bg-dark" tabindex="-1" id="offcanvasDarkNavbar" aria-labelledby="offcanvasDarkNavbarLabel">  
                <div class="offcanvas-header">
                    




                  <h5 class="offcanvas-title" id="offcanvasDarkNavbarLabel"></h5>
                  <button type="button" class="btn-close btn-close-white" data-bs-dismiss="offcanvas" aria-label="Close"></button>
                </div>
                
                <div class="offcanvas-body">
                  <!--<ul class="navbar-nav justify-content-end flex-grow-1 pe-3">-->
                  <ul class="navbar-nav justify-content flex-grow-1 pe-3">  
                    
                    <li class="nav-item">
                      <a class="nav-link active" aria-current="page" href="{{url_for('principal')}}">Home</a>
                    </li>
                    
                    
                    <li class="nav-item dropdown">
                      <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                        Chart Types
                      </a>
                      <ul class="dropdown-menu dropdown-menu-dark">
                        <li><a class="dropdown-item" href="{{url_for('linecharts')}}">Line Chart</a></li>
                        <li><a class="dropdown-item" href="{{url_for('areacharts')}}">Area Charts</a></li>
                        <li><a class="dropdown-item" href="{{url_for('columncharts')}}">Column Charts</a></li>
                        <li><a class="dropdown-item" href="{{url_for('barcharts')}}">Bar Charts</a></li>
                        <li><a class="dropdown-item" href="{{url_for('combocharts')}}">Mixed / Combo Charts</a></li>
                        <li><a class="dropdown-item" href="{{url_for('rangecharts')}}">Range Area Charts</a></li>
                        <li><a class="dropdown-item" href="{{url_for('timelinecharts')}}">Timeline Charts</a></li>
                        <li><a class="dropdown-item" href="{{url_for('funnelcharts')}}">Funnel Charts</a></li>
                        <li><a class="dropdown-item" href="{{url_for('candlestickcharts')}}">Candlestick Charts</a></li>
                        <li><a class="dropdown-item" href="{{url_for('boxcharts')}}">Box & Wisker Charts</a></li>
                        <li><a class="dropdown-item" href="{{url_for('piecharts')}}">Pie / Donuts Charts</a></li>
                        <li><a class="dropdown-item" href="{{url_for('radarcharts')}}">Radar Charts</a></li>
                        <li><a class="dropdown-item" href="{{url_for('polarcharts')}}">Polar Area Charts</a></li>
                        <li><a class="dropdown-item" href="{{url_for('radialcharts')}}">RadialBars / Circle Charts</a></li>
                        <li><a class="dropdown-item" href="{{url_for('bubblecharts')}}">Bubble Charts</a></li>
                        <li><a class="dropdown-item" href="{{url_for('scattercharts')}}">Scatter Charts</a></li>
                        <li><a class="dropdown-item" href="{{url_for('heatmapcharts')}}">Heatmap Charts</a></li>
                        <li><a class="dropdown-item" href="{{url_for('treemapcharts')}}">Treemap Charts</a></li>
                        

                      </ul>
                    </li>
                  </ul>
                  
                  <form class="d-flex mt-3" role="search">
                    <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
                    <button class="btn btn-success" type="submit">Search</button>
                  </form>
                
                </div>
              </div>
            </div>
          </nav>

     
        <br>
        <br>
        <br>
        <br>
        <br>

        <!-- Main content area -->

        <div id="main-content">
    
          <div class="row row-cols-3">
            <div class="col-2"></div>
              <div class="col-8">
                <h1 style = 'margin-left:10px;margin-bottom:20px;'>Line Chart Straight</h1>
              </div>
            <div class="col-2"></div>
          </div>
        
          <div class="row row-cols-3">
            <div class="col-2"></div>
            <div class="col-8 border border-primary rounded-2" id="real_time_line"></div>
            <div class="col-2"></div>
          </div>
        
        
        </div>















        <!-- Main content area -->



    
 
        <footer class="mt-5 bg-dark text-center text-light p-4">
     
          <a href="https://github.com/eurico3" target="_blank" id="gitlogo"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="rgb(108,198,68)" class="bi bi-github" viewBox="0 0 16 16">
            <path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27s1.36.09 2 .27c1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.01 8.01 0 0 0 16 8c0-4.42-3.58-8-8-8"/>
          </svg></a>
        <a href="https://www.linkedin.com/in/euricopaes" target="_blank"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="rgb(0,119,181)" class="bi bi-linkedin" viewBox="0 0 16 16">
            <path d="M0 1.146C0 .513.526 0 1.175 0h13.65C15.474 0 16 .513 16 1.146v13.708c0 .633-.526 1.146-1.175 1.146H1.175C.526 16 0 15.487 0 14.854zm4.943 12.248V6.169H2.542v7.225zm-1.2-8.212c.837 0 1.358-.554 1.358-1.248-.015-.709-.52-1.248-1.342-1.248S2.4 3.226 2.4 3.934c0 .694.521 1.248 1.327 1.248zm4.908 8.212V9.359c0-.216.016-.432.08-.586.173-.431.568-.878 1.232-.878.869 0 1.216.662 1.216 1.634v3.865h2.401V9.25c0-2.22-1.184-3.252-2.764-3.252-1.274 0-1.845.7-2.165 1.193v.025h-.016l.016-.025V6.169h-2.4c.03.678 0 7.225 0 7.225z"/>
          </svg></a>
      </footer>

    <!-- Apex assets scripts on bottom of code-->
    <script>


var lastDate = 0;
var data = []
var TICKINTERVAL = 86400000
// Range Eixo x e definido aqui - por exemplo 77760000 equivale a 6 dias 
let XAXISRANGE = 777600000


function getDayWiseTimeSeries(baseval, count, yrange) {
  var i = 0;
  while (i < count) {
    var x = baseval;
    var y = Math.floor(Math.random() * (yrange.max - yrange.min + 1)) + yrange.min;

    data.push({
      x, y
    });
    lastDate = baseval
    baseval += TICKINTERVAL;
    i++;
  }
}

getDayWiseTimeSeries(new Date('11 Feb 2017 GMT').getTime(), 10, {
  min: 10,
  max: 90
})

function getNewSeries(baseval, yrange) {
  var newDate = baseval + TICKINTERVAL;
  lastDate = newDate
/*
  for(var i = 0; i< data.length - 10; i++) {
    // IMPORTANT
    // we reset the x and y of the data which is out of drawing area
    // to prevent memory leaks
    data[i].x = newDate - XAXISRANGE - TICKINTERVAL
    data[i].y = 0
  }
*/
  data.push({
    x: newDate,
    y: Math.floor(Math.random() * (yrange.max - yrange.min + 1)) + yrange.min
    //y: 50
  })
  console.log(data)
}





///////////////////

var real_time_options = {
  series: [{
  //data: data.slice()
  data: data
}],
  chart: {
  id: 'realtime',
  height: 350,
  type: 'line',
//  animations: {
//    enabled: true,
//    easing: 'linear',
//    dynamicAnimation: {
//      speed: 1000
//    }
//  },
  toolbar: {
    show: false
  },
  zoom: {
    enabled: false
  }
},
dataLabels: {
  enabled: false
},
stroke: {
  curve: 'smooth'
},
title: {
  text: 'Dynamic Updating Chart',
  align: 'left'
},
markers: {
  size: 0
},
xaxis: {
  type: 'datetime',
  range: XAXISRANGE,
},
yaxis: {
  max: 100
},
legend: {
  show: false
},
};

var real_chart = new ApexCharts(document.querySelector("#real_time_line"), real_time_options);
real_chart.render();


window.setInterval(function () {
getNewSeries(lastDate, {
  min: 10,
  max: 90
})

  real_chart.updateSeries([{
    data: data
  }])
  }, 1000)
/*
  window.setInterval(function () {
getNewSeries(lastDate, {
  min: 10,
  max: 90
})

}, 1000)
*/


    </script>
    <!-- Bootstrap Javascript Bundle-->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>
    
    <!-- Bootstrap popover and tooltip-->
    <script>
      const popoverTriggerList = document.querySelectorAll('[data-bs-toggle="popover"]')
      const popoverList = [...popoverTriggerList].map(popoverTriggerEl => new bootstrap.Popover(popoverTriggerEl))

      const tooltipTriggerList = document.querySelectorAll('[data-bs-toggle="tooltip"]')
      const tooltipList = [...tooltipTriggerList].map(tooltipTriggerEl => new bootstrap.Tooltip(tooltipTriggerEl))
    </script>



</body>
</html>

