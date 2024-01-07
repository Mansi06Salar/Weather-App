# Weather-App(Using HTML,CSS and JavaScript)


<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>My Weather APP</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-4bw+/aepP/YC94hEpVNVgiZdgIC5+VKNBQNGCHeKRQN+PtmoHDEXuppvnDJzQIu9" crossorigin="anonymous">
  </head>
  <body>
    <nav class="navbar navbar-expand-lg bg-body-tertiary">
      <div class="container-fluid">



        <a class="navbar-brand" href="#">Weather App</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#">Home</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">About this App</a>
            </li>
            <li class="nav-item dropdown">
              <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                
              </a><ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">Delhi</a></li>
                <li><a class="dropdown-item" href="#">Seattle</a></li>
                <li><hr class="dropdown-divider"></li>
                <li><a class="dropdown-item" href="#">Banglore</a></li>
              </ul>
              
            </li>
            <li class="nav-item">
              <a class="nav-link">Usage Guide</a>
            </li>
          </ul>
          <form class="d-flex" role="search">
            <input id="city" type="search" placeholder="Search" aria-label="Search">
            <button class="btn btn-outline-success" type="submit" id="submit">Search</button>
          </form>
        </div>
      </div>
    </nav>


    <div class="container">
      <h1 class="my-4 text-center">Weather for <span id="cityName"></span></h1>
      <main>
        <div class="row row-cols-1 row-cols-md-3 mb-3 text-center">
          <div class="col">
            <div class="card mb-4 rounded-3 shadow-sm">
              <div class="card-header py-3">
                <h4 class="my-0 fw-normal">Temperature</h4>
              </div>
              <div class="card-body">
                <h1 class="card-title pricing-card-title"><sup>&deg</sup><small class="text-body-secondary fw-light"></small><span id="temp2"></span>>C</small></h1>
                <ul class="list-unstyled mt-3 mb-4">
                  <li>Temperature is <span id="temp"></span></li>
                  <li>Min temperature is <span id="min_temp"></span></li>
                  <li>Max temperature is <span id="max_temp"></span></li>
                  
                </ul>
                <button type="button" class="w-100 btn btn-lg btn-outline-primary"></button>
              </div>
            </div>
          </div>
          <div class="col">
            <div class="card mb-4 rounded-3 shadow-sm">
              <div class="card-header py-3">
                <h4 class="my-0 fw-normal">Humidity Info</h4>
              </div>
              <div class="card-body">
                <h1 class="card-title pricing-card-title"><span id="humidity2"></span><small class="text-body-secondary fw-light">%</small></h1>
                <ul class="list-unstyled mt-3 mb-4">
                  <li>Wind Degree <span id="wind_degrees"></span></li>
                  <li>Feels Like <span id="feels_like"></span></li>
                  <li>Humidity is <span id="humidity"></span></li>
                </ul>
                <button type="button" class="w-100 btn btn-lg btn-primary"></button>
              </div>
            </div>
          </div>
          <div class="col">
            <div class="card mb-4 rounded-3 shadow-sm border-primary">
              <div class="card-header py-3 text-bg-primary border-primary">
                <h4 class="my-0 fw-normal">Wind info</h4>
              </div>
              <div class="card-body">
          <h1 class="card-title pricing-card-title"><span id="wind_speed2"></span><small class="text-body-secondary fw-light">km/hr</small></h1>
                <ul class="list-unstyled mt-3 mb-4">
                  
                  <li>Wind Speed is <span id="wind_speed"></span></li>
                  <li>Sunrise Time is <span id="sunrise"></span></li>
                  <li>Sunset Time is <span id="sunset"></span></li>
                  
                </ul>
                <button type="button" class="w-100 btn btn-lg btn-primary"></button>
              </div>
            </div>
          </div>
        </div>
    
        <h2 class="display-6 text-center mb-4">Weather of other common places</h2>
    
        <div class="table-responsive">
          <table class="table text-center">
            <thead>
              <tr>
                <th style="width: 34%;"></th>
                <th style="width: 22%;">CLOUD_PCT</th>
<th style="width: 22%;">FEELS_LIKE</th>
<th style="width: 22%;">HUMIDITY</th>
<th style="width: 22%;">MAX_TEMP</th>
<th style="width: 22%;">MIN_TEMP</th>
<th style="width: 22%;">SUNRISE</th>
<th style="width: 22%;">SUNSET</th>
<th style="width: 22%;">TEMP</th>
<th style="width: 22%;">WIND_DEGREES</th>
<th style="width: 22%;">WIND_SPEED</th>

              </tr>
            </thead>
            <tbody>
              <tr>
                <th scope="row" class="text-start">Shanghai</th>
                <td>1</td>
                <td>2</td>
                <td>3</td>
                <td>4</td>
                <td>5</td>
                <td>1</td>
                <td>2</td>
                <td>3</td>
                <td>4</td>
                <td>5</td>
              </tr>
              <tr>
                <th scope="row" class="text-start">Boston</th>
                <td>1</td>
                <td>2</td>
                <td>3</td>
                <td>4</td>
                <td>5</td>
                <td>1</td>
                <td>2</td>
                <td>3</td>
                <td>4</td>
                <td>5</td>
              </tr>
            </tbody>
    
            <tbody>
              <tr>
                <th scope="row" class="text-start">Lucknow</th>
                <td>1</td>
                <td>2</td>
                <td>3</td>
                <td>4</td>
                <td>5</td>
                <td>1</td>
                <td>2</td>
                <td>3</td>
                <td>4</td>
                <td>5</td>
                
              </tr>
              <tr>
                <th scope="row" class="text-start">Kolkata</th>
                <td>1</td>
                <td>2</td>
                <td>3</td>
                <td>4</td>
                <td>5</td>
                <td>1</td>
                <td>2</td>
                <td>3</td>
                <td>4</td>
                <td>5</td>
              </tr>
              <tr>
                <th scope="row" class="text-start">Mumbai</th>
                <td>1</td>
                <td>2</td>
                <td>3</td>
                <td>4</td>
                <td>5</td>
                <td>1</td>
                <td>2</td>
                <td>3</td>
                <td>4</td>
                <td>5</td>
              </tr>
              <tr>
                <th scope="row" class="text-start">Rajasthan</th>
                <td>1</td>
                <td>2</td>
                <td>3</td>
                <td>4</td>
                <td>5</td>
                <td>1</td>
                <td>2</td>
                <td>3</td>
                <td>4</td>
                <td>5</td>
              </tr>
            </tbody>
          </table>
        </div>
      </main>
    </div>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/js/bootstrap.bundle.min.js" integrity="sha384-HwwvtgBNo3bZJJLYd8oVXjrBZt8cqVSpeBNS5n7C8IVInixGAoxmnlMuBnhbgrkm" crossorigin="anonymous"></script>
    <script src="script.js"></script>
  </body>
</html>
