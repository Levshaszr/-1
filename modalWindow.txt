<!-- html -->
<html>
  <head>
    <title>Title</title>
  </head>
  <body>
    <a href="#modalWindow" class="button">Open</a>
    <div id="modalWindow">
      <div class="window">
        <p>Cool</p>
        <a href="#close" class="close">x</a>
      </div>
    </div>
  </body>
</html>
<!-- end html -->

<!-- css -->
#modalWindow {
  position: absolute;
  left: 0;
  top: 0;
  background: rgba(0, 0, 0, 0.7);
  width: 100%;
  height: 100%;
  display: none;
  pointer-events: none;
  -webkit-animation: animationModal .5s;
    -moz-animation: animationModal .5s;
      -ms-animation: animationModal .5s;
         -o-animation: animationModal .5s;
            animation: animationModal .5s;
}
#modalWindow:target {
  pointer-events: auto;
  display: block;
}
.window {
  width: 300px;
  min-height: 100px;
  height: auto;
  background: #f00;
  margin: 30% auto;
  border-radius: 5px;
  z-index: 9999;
  padding: 10px;
}
.close {
  position: absolute;
  right: 5px;
  top: 5px;
  background: #fff;
  color: #000;
  text-decoration: none;
  padding: 2px 10px 5px 10px;
  border-radius: 50%;
  
  -webkit-transition: .5s;
    -moz-transition: .5s;
      -ms-transition: .5s;
        -o-transition: .5s;
          transition: .5s;
}
.close:hover {
  color: red;
}
@-webkit-keyframes animationModal {
  0% {
    -webkit-transform: scale(0.5);
  }
  100% {
     -webkit-transform: scale(1);
  }
}
<!-- end css -->