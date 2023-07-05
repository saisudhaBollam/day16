<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CallBack-Hell</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.6.1/dist/css/bootstrap.min.css" integrity="sha384-zCbKRCUGaJDkqS1kPbPd7TveP5iyJE0EjAuZQTgFLD2ylzuqKfdKlfG/eSrtxUkn" crossorigin="anonymous">
    <link rel="stylesheet" href="style.css">
</head>
<body>
     <div class="container">
         <section id="timer">
            <div class="row" id="timer-content"> 
                <div class="col-xs-12 col-sm-12 col-md-12 countdown-wrapper text-center">
                    <div class="card">
                        <div class="card-header">
                            Count Down
                        </div>
                        <div class="card-block">
                            <div id="countdown">
                                <span id="sec" class="timer bg-primary"></span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div id="wishes-content" class="col-xs-12 col-sm-12 col-md-12 text-center" style="display: none;">
                <p><span class="multicolortext">Happy Independence Day</span></p>
                <img src="images/Independance_day_img.jpg"class="img-fluid rounded" alt="Responsive image" height="550" width="550"/>
            </div>
         </section>
     </div>  
     <script src="https://cdn.jsdelivr.net/npm/jquery@3.5.1/dist/jquery.slim.min.js" integrity="sha384-DfXdz2htPH0lsSSs5nCTpuj/zy4C+OGpamoFVy38MVBnE+IbbVYUew+OrCXaRkfj" crossorigin="anonymous"></script>
<script src="https://cdn.jsdelivr.net/npm/bootstrap@4.6.1/dist/js/bootstrap.bundle.min.js" integrity="sha384-fQybjgWLrvvRgtW6bFlB7jaZrFsaBXjsOMm/tB9LTS58ONXgqbR9W8oWht/amnpF" crossorigin="anonymous"></script>
    <script src="script.js"></script>
</body>
</html>
 36 changes: 36 additions & 0 deletions36  
script.js
@@ -0,0 +1,36 @@
let countdown = 10;
var timer = document.getElementById('sec');
timer.innerHTML = countdown--;
setTimeout(() => {
    timer.innerText = countdown--;
    setTimeout(() => {
        timer.innerText = countdown--;
        setTimeout(() => {
            timer.innerText = countdown--;
            setTimeout(() => {
