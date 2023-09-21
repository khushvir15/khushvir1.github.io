# khushvir1.github.io

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible"
  content="ie=edge">
  <!-- Latest compiled and minified CSS -->
<!--<link rel="stylesheet" href="css/bootstrap.css">
<link rel="stylesheet" href="css/bootstrap.min.css"> -->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-alpha.6/css/bootstrap.min.css"
integrity="sha384-rwoIResjU2yc3z8GV/NPeZWAv56rSmLldC3R/AZzGRnGxQQKnKkoFVhFQhNUwEyJ" crossorigin="anonymous">

  <style>
  body{
    margin-top: 70px;
    background: lightblue;
    color: brown;
  }
  </style>

  <title>Weight Convertor</title>

</head>

<body>
  <div class="container">
    <div class="row">
      <div class="col-md-6 offset-md-3">
        <h1 class="display-4 text-center mb-3"> Weight Converter</h1>
        <form>
          <div class="form-group">
            <input id="kgInput" type="number"
            class="form-control form-control-lg mb-3"
            placeholder="Enter Kilograms....">

            <div>
            <input id="btn1" value="Go" type="button" name="Go" color="black"  class="btn button-danger offset-md-5 mb-1"/>
            </div>
          </div>
        </form>

        <div id="output">

          <div class="card card-primary mb-2">
            <div class="card-block">
              <h4>Pounds: </h4>
              <div id="lbsOutput"></div>
            </div>
          </div>

          <div class="card card-success mb-2">
            <div class="card-block">
              <h4>Ounces: </h4>
              <div id="ozOutput"></div>
            </div>
          </div>

          <div class="card card-danger mb-2">
            <div class="card-block">
              <h4>Grams: </h4>
              <div id="gramsOutput"></div>
            </div>
          </div>


        </div>
      </div>
    </div>
  </div><br><br>
<!--<div><center>If you want to convert length than click on the button given below:</center><br>
<a href="Length Converter.html">
<center><button type="button" class="btn btn-warning"><h4>Length Converter</h4></button></center></a>
</div>-->
<script>

document.getElementById('kgInput').addEventListener('input',
function(e){
  let kgs = e.target.value;
  document.getElementById('btn1').addEventListener('click',function(){
  document.getElementById('lbsOutput').innerHTML= (kgs*2.20462).toFixed(2);
  document.getElementById('ozOutput').innerHTML = (kgs*35.274).toFixed(2);
  document.getElementById('gramsOutput').innerHTML= (kgs*1000).toFixed(0);
  });
});

</script>
</body>
</html>
