# Snap-Editor
Hey, myself Pranav Gotawala recently i have created snap editor check out this poject and drag and drop your img n try to edit. thankyou 
<!DOCTYPE html>
<html lang="en" style="background-color: rgb(0, 0, 0); text-decoration: none; color: white;" id="html">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="C:\Users\Owner\node_modules\cropperjs\src\css\cropper.css">
    <link rel="stylesheet" href="D:\.vscode\snap editor\snap.css">
  <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.6.3/css/all.css" integrity="sha384-UHRtZLI+pbxtHCWp1t77Bi1L4ZtiqrqD80Kn4Z8NTSRyMA2Fd33n5dQ8lWUE00s/" crossorigin="anonymous"></head>
    <title>Snap | Pranav Gotawala</title>
</head>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Coda+Caption:wght@800&display=swap');

* {
    margin:  0;
    padding: 0;
    box-sizing: border-box;
    outline: none;
}

html {
    user-select: none;
    overflow-x: hidden;
}

img {
    max-width: 100%;
    max-height: 100%;
    top: 50%;
    left: 50%;
    transform: translateX(-50%) translateY(-50%);
    position: fixed;
}
input {
    height: 3rem;
    width: 30rem;
    margin: 1rem;
    border-radius: 20px;
    box-shadow: 0 0 18px 0 white;
}
input[type=text] {
    font-size: 1rem;
    padding-left: 2rem;
    font-weight: 900;
    font-family: 'Coda Caption', sans-serif;
}
.top {
    background-color: rgb(0, 0, 0);
}
.right-icons {
    background-color: rgb(255, 0, 0);
    text-decoration: none;
}
.right-icons ul {
    font-size: 35px;
    position: fixed;
    right: 1rem;
    list-style: none;
    margin: 2rem;
    top: 1rem;
}
.right ul li {
    margin: 2rem 0 0 0;
    background-color: transparent;
    width: 5rem;
    height: 5rem;
    border-radius: 50%;
    text-align: center;
    padding: 1.4rem 0 0 0;
    transition: 0.6s;
    color: violet;
    box-shadow: 0 0 10px 0 white;
    cursor: pointer;
}

ul li {
    margin: 2rem 0 0 0;
    background-color: transparent;
    width: 5rem;
    height: 5rem;
    border-radius: 50%;
    text-align: center;
    padding: 1.4rem 0 0 0;
    transition: 0.6s;
    color: violet;
    box-shadow: 0 0 10px 0 white;
    cursor: pointer;   
}

ul li:hover {
    background-color: rgb(228, 228, 228, 0.5);
    transform: rotate(360deg);
    
}
.left-icons ul {
    font-size: 35px;
    position: fixed;
    left: 1rem;
    list-style: none;
    margin: 2rem;
    top: 1rem;
}

.mystyle {
    background-color: rgb(255, 255, 255);
    transition: .5s;
    transform: rotate(360deg);
  }
  .mystyle:hover {
      background-color: rgb(228, 228, 228, 0.5);
  }
  .right {
    background-color: rgb(255, 255, 255);
    transition: .5s;
    transform: rotate(360deg);
  }
  .right:hover {
    background-color: rgb(228, 228, 228, 0.5);
}
 .box {
     border: 3px dotted rgb(255, 255, 255, 0.5);
     width: 900px;
     height: 500px;
     position: fixed;
     left: 50%;
     top: 50%;
     transform: translateX(-50%) translateY(-50%);
     text-align: center;

 }
  .box h1 {
     font-size: 2rem;
     margin-top: 40%;
     opacity: 0.3;
     border: 3px dotted white;
     padding: 0.5rem;
     font-family: 'Coda Caption', sans-serif;

 } 
 .close {
     position: fixed;
     width: 2rem;
     height: 2rem;
     left: 50%;
     transform: translateX(-50%);
     background-color: white;
     top: -2rem;
     border-radius: 50%;
 }
.search {
    background-color: white;
    width: 100%;
    height: 100%;
    position: fixed;
    z-index: 1;
}

.loadingnext {
    margin-top: 10rem;
}
.loadingthi {
    margin-top: 20rem;
}
.first {
    border: 5px dotted black;
    background-color: transparent;
    position: absolute;
    margin: 5rem;
    width: 3rem;
    height: 3rem;
    border-radius: 50%;
    margin-left: 4rem;
}
.sec {
    border: 5px dotted black;
    background-color: transparent;
    position: absolute;
    margin: 5rem;
    width: 3rem;
    height: 3rem;
    border-radius: 50%;
    margin-left: 19rem;
}
.thi {
    border: 5px dotted black;
    background-color: transparent;
    position: absolute;
    margin: 5rem;
    width: 3rem;
    height: 3rem;
    border-radius: 50%;
    margin-left: 34rem;
}
.for {
    border: 5px dotted black;
    background-color: transparent;
    position: absolute;
    margin: 5rem;
    width: 3rem;
    height: 3rem;
    border-radius: 50%;
    margin-left: 49rem;
}
.fiv {
    border: 5px dotted black;
    background-color: transparent;
    position: absolute;
    margin: 5rem;
    width: 3rem;
    height: 3rem;
    border-radius: 50%;
    margin-left: 64rem;
}
.six {
    border: 5px dotted black;
    background-color: transparent;
    position: absolute;
    margin: 5rem;
    width: 3rem;
    height: 3rem;
    border-radius: 50%;
    margin-left: 79rem;
}
#urll {
   margin-top: 20%;
   margin-left: 32%;
   position: fixed;
   z-index: 1;
}
#slide {
    background-color: rgba(162, 188, 236, 0.5);
    width: 100%;
    height: 100%;
    position: fixed;
    z-index: 1;
    transform: translateX(-90rem);
}
#srcc {
    position: fixed;
}
#srcc:hover {
    box-shadow: 0 0 10px 0 white;
    opacity: 0.8;
    transition: 300ms;
}
#sli:hover {
    opacity: 0.8;
    box-shadow: 0 0 8px 0 white;
}
#pop {
    background-color: black;
    width: 3rem;
    height: 3rem;
    border-radius: 50%;
    position: absolute;
    right: 2rem;
    top: 1rem;
    box-shadow: 0 0 18px 0 black;
}
#pop:hover {
    box-shadow: 0 0 18px 0 crimson;
    transition: .5s;
}
#songslist {
    background-color:rgb(251, 156, 118,0.9);
    width: 100%;
    height: 100%;
    z-index: 1;
    position: fixed;
}
#popp {
    background-color: black;
    width: 3rem;
    height: 3rem;
    border-radius: 50%;
    position: absolute;
    right: 2rem;
    top: 1rem;
    box-shadow: 0 0 18px 0 black;
}
#poop {
    background-color: black;
    width: 3rem;
    height: 3rem;
    border-radius: 50%;
    position: absolute;
    right: 2rem;
    top: 1rem;
    box-shadow: 0 0 18px 0 black;
}
#poop:hover {
    box-shadow: 0 0 18px 0 crimson;
    transition: .5s;
}

#popp:hover {
    box-shadow: 0 0 18px 0 crimson;
    transition: .5s;
}
#seconds {
    background-color: rgba(10, 1, 1, 0.8);
    z-index: 1;
    width: 100%;
    min-height: 100vh;
    position: absolute;  
}
#sec {
    text-align: center;
    font-size: 10rem;
    margin-top: 15rem;
}
.bar {
    background-color: rgb(211, 107, 32,0.8);
    width: 100%;
    height: 11.5rem;
    position: absolute;
    z-index: -1;
}
.n0 {
    transition: .5s;
}
.n1 {
    transition: .5s;
}
.n2 {
    transition: .5s;
}
.n3 {
    transition: .5s;
}
.n4 {
    transition: .5s;
}
.n5 {
    transition: .5s;
}
.inff {
    transition: .5s;
}
.n0:hover {
    background-color: rgb(165, 165, 165,0.5);
}
.n1:hover {
    background-color: rgb(165, 165, 165,0.5);
}
.n2:hover {
    background-color: rgb(165, 165, 165,0.5);
}
.n3:hover {
    background-color: rgb(165, 165, 165,0.5);
}
.n4:hover {
    background-color: rgb(165, 165, 165,0.5);
}
.n5:hover {
    background-color: rgb(165, 165, 165,0.5);
}
.inff:hover {
    background-color: rgb(165, 165, 165,0.5);
}
#canvas {
    cursor: crosshair;
    top: 50%;
    left: 50%;
    transform: translateX(-50%) translateY(-50%);
    position: absolute;
}
button {
    position: absolute;
    width: 5rem;
    height: 2rem;
    border-radius: 30px;
    background-color: red;
    transition: 300ms;
    transform: translateX(35rem) translateY(-2.5rem);
}
#container {
    width: 900px;
    height: 500px;
    background-color: transparent;
    border: 5px solid green;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 7px;
    touch-action: none;
    top: 50%;
    left: 50%;
    transform: translateY(-50%) translateX(-50%);
    z-index: 1;
    position: fixed;
  }

  #item {
    width: 200px;
    height: 200px;
    border: 5px solid red;
    touch-action: none;
    user-select: none;
  }
  #item:hover {
      cursor: grab ;
  }
button:hover {
    opacity: 0.8;
}
 @media screen and (max-width: 1100px) {
    html {
        zoom: 69%;
    }
 }
</style>
<body>

    <meta name="viewport" 
          content="width=device-width, 
          initial-scale=1.0, 
          user-scalable=no" />
    <style>
      #container {
        width: 900px;
        height: 500px;
        background-color: transparent;
        display: flex;
        align-items: center;
        justify-content: center;
        overflow: hidden;
        touch-action: none;
      }
      #item {
        width: 300px;
        height: 300px;
        background-color: transparent;
        border: 10px solid red;
        touch-action: none;
        user-select: none;
      }
      #item:hover {
        cursor: grab;
      }
    </style>
  </head>
  
  <body>
  
    <div id="outerContainer">
      <div id="container">
        <div id="item">
  
        </div>
      </div>
    </div>
  
    <script>
      var dragItem = document.querySelector("#item");
      var container = document.querySelector("#container");
  
      var active = false;
      var currentX;
      var currentY;
      var initialX;
      var initialY;
      var xOffset = 0;
      var yOffset = 0;
  
      container.addEventListener("touchstart", dragStart, false);
      container.addEventListener("touchend", dragEnd, false);
      container.addEventListener("touchmove", drag, false);
  
      container.addEventListener("mousedown", dragStart, false);
      container.addEventListener("mouseup", dragEnd, false);
      container.addEventListener("mousemove", drag, false);
  
      function dragStart(e) {
        if (e.type === "touchstart") {
          initialX = e.touches[0].clientX - xOffset;
          initialY = e.touches[0].clientY - yOffset;
        } else {
          initialX = e.clientX - xOffset;
          initialY = e.clientY - yOffset;
        }
  
        if (e.target === dragItem) {
          active = true;
        }
      }
  
      function dragEnd(e) {
        initialX = currentX;
        initialY = currentY;
  
        active = false;
      }
  
      function drag(e) {
        if (active) {
        
          e.preventDefault();
        
          if (e.type === "touchmove") {
            currentX = e.touches[0].clientX - initialX;
            currentY = e.touches[0].clientY - initialY;
          } else {
            currentX = e.clientX - initialX;
            currentY = e.clientY - initialY;
          }
  
          xOffset = currentX;
          yOffset = currentY;
  
          setTranslate(currentX, currentY, dragItem);
        }
      }
  
      function setTranslate(xPos, yPos, el) {
        el.style.transform = "translate3d(" + xPos + "px, " + yPos + "px, 0)";
      }
    </script>
  <button id="btn" class="bttn">Clear</button>
  <canvas id="canv" width="900" height="500" style="position:absolute; top:4.8rem; left:14.45rem; border: red 3px solid; z-index: 1;"></canvas>
<div id="seconds" style="transform: translateX(-200rem);">
  <div id="poop"><i class="fas fa-times" style="color: rgb(255, 0, 0); font-size: 2rem; position: fixed; right: 2.85rem; top: 1.5rem;"></i></div>
  <div id="sec">
        <ol>
          <div class="bar" id="barr"></div>
          <li class="n0" id="no0">0</li><br>
          <li class="n1" id="no1">1</li><br>
          <li class="n2" id="no2">2</li><br>
          <li class="n3" id="no3">3</li><br>
          <li class="n4" id="no4">4</li><br>
          <li class="n5" id="no5">5</li><br>
          <li class="inff" id="iff">Infinite</li>
        </ol>
  </div>
</div>


  <div id="slide">
    <div id="pop"><i class="fas fa-times" style="color: rgb(255, 0, 0); font-size: 2rem; position: fixed; right: 2.85rem; top: 1.5rem;"></i></div>
    <div id="urll" >
      <input type="text" style="width: 25rem; box-shadow: 0 0 18px 0 black;" placeholder="Type a URL" id="url"><i class="fas fa-search" id="srcc" style="font-size: 2rem; background-color:
      rgb(130, 168, 238); width: 3.5rem; height: 3.5rem; transform: translateY(10px) translateX(-8px); border-radius: 50%; padding: 0.65rem;"></i>
    </div>
  </div>


<div id="songslist" style="overflow-y: scroll; transform: translateX(90rem);">
  <div id="popp"><i class="fas fa-times" style="color: rgb(255, 0, 0); font-size: 2rem; position: fixed; right: 2.85rem; top: 1.5rem;"></i></div>
  <h1 style="font-family:Cambria, Cochin, Georgia, Times, 'Times New Roman', serif; font-size: 3rem; letter-spacing: 2px; text-align: center; margin-top: 0.5rem;">Music</h1><br><hr><br>
  <h2 style="font-family: 'Coda Caption', sans-serif; margin: 1rem;">Trending</h2>
  <iframe src="https://open.spotify.com/embed/track/1Bhm5HNO1cq8olDbBmokyL" width="300" height="380" style="margin: 1rem;" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe> <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/4iJyoBOLtHqaGxP12qzhQI" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe> <iframe  style="margin: 1rem;" src="https://open.spotify.com/embed/track/3VT8hOC5vuDXBsHrR53WFh" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe> <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/1J14CdDAvBTE1AJYUOwl6C" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe> <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/3H3r2nKWa3Yk5gt8xgmsEt" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/0lx2cLdOt3piJbcaXIV74f" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/0t1kP63rueHleOhQkYSXFY" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/6moU77g9RQyMzHNuKEaQKq" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/6UelLqGlWMcVH1E5c4H7lY" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/5ZKG94fnjiuMH5yrC5S9lS" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/3ee8Jmje8o58CHK66QrVC2" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/285pBltuF7vW8TeWk8hdRR" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/1TwbzKMxFBExaDEUWqQ832" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/7dt6x5M1jzdTEt8oCbisTK" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/41L3O37CECZt3N7ziG2z7l" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/4umIPjkehX1r7uhmGvXiSV" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/1Sl3njkhhz8nrSPZroDQ82" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/2G7V7zsVDxg1yRsu7Ew9RJ" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/7FEwp8BavoEVE3AnxJDchc" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/2wrJq5XKLnmhRXHIAf9xBa" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/2P91MQbaiQOfbiz9VqhqKQ" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/3Dv1eDb0MEgF93GpLXlucZ" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/0tgVpDi06FyKpA1z0VMD4v" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/5WHTFyqSii0lmT9R21abT8" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/2iUXsYOEPhVqEBwsqP70rE" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/2l8w0zZVn4AZNuzrht7MRT" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/37FXw5QGFN7uwwsLy8uAc0" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/2rRJrJEo19S2J82BDsQ3F7" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/2tnVG71enUj33Ic2nFN6kZ" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/7fa9MBXhVfQ8P8Df9OEbD8" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/1SyjFJu9xk5CpYD6bm1tjl" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
  <iframe style="margin: 1rem;" src="https://open.spotify.com/embed/track/1M4qEo4HE3PRaCOM7EXNJq" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
</div>
    <div class="search" id="ser">
    <div class="top">
      <i class="fas fa-times" id="cls" style="font-size: 2rem; background-color: transparent; width: 3.5rem; height: 3.5rem;
      border: 3px solid white; transform: translateX(81rem) translateY(12px); padding: 10px 13px 10px; position: fixed;"></i>
        <input type="text" id="input" placeholder="Search"><i class="fas fa-search" id="src" style="font-size: 2rem; background-color:
         violet; width: 3.5rem; height: 3.5rem; border-radius: 50%;transform: translateY(2px) translateX(-8px); padding: 0.65rem;"></i>
        <hr>
    </div>
        <div class="loading" id="load">  
          <p class="first"></p>
          <p class="sec"></p>
          <p class="thi"></p>
          <p class="for"></p>
          <p class="fiv"></p>
          <p class="six"></p>
        </div>
        <div class="loadingnext">  
            <p class="first" id="f"></p>
            <p class="sec" id="s"></p>
            <p class="thi" id="t"></p>
            <p class="for" id="fo"></p>
            <p class="fiv" id="fi"></p>
            <p class="six" id="si"></p>
          </div>
          <div class="loadingthi">  
            <p class="first" id="fs"></p>
            <p class="sec" id="se"></p>
            <p class="thi" id="th"></p>
            <p class="for" id="fr"></p>
            <p class="fiv" id="fv"></p>
            <p class="six" id="sx"></p>
          </div>
    </div>
    <img src="" alt="" id="img">
    <div class="close" onclick="close()"><i class="fas fa-times" style="font-size: 1rem; padding: 0.5rem; margin-left: 0.15rem; color: rgb(0, 0, 0);"></i></div><p id="demo"></p>
    <div class="box" id="dropzone"><i class="fas fa-plus-circle"
 style="color: rgba(255, 255, 255, 0.2); cursor: pointer; font-size: 8rem; position: fixed; top: 50%; left: 50%; transform: translateX(-50%) translateY(-50%);"></i><h1 id="h1">Drag your image here and edit it.</h1>
</div>
<div class="right-icons" id="right" style="position: fixed; right: 1rem;">
    <ul>
    <li id="text" onclick="mytext()"><i class="fas fa-text-height"></i></li>
    <li id="pen" onclick="mypen()"><i class="fas fa-pen"></i></li>
    <li id="music"><i class="fas fa-music"></i></li>
    <li id="crop" onclick="mycrop()"><i class="fas fa-crop-alt"></i></li>
</ul>
</div>
<div class="left-icons" id="left" style="position: fixed;">
    <ul>
    <li id="cut"><i class="fas fa-cut"></i></li>
    <li id="find"><i class="fas fa-search"></i></li>
    <li id="link"><i class="fas fa-link"></i></li>
    <li id="infi"><i class="fas fa-infinity"></i></li>
</ul>
</div>
</body>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.1/jquery.min.js"></script>
<script>

//draw canvas


class SignTool {
  constructor() {
    this.initVars()
    this.initEvents()
  }

  initVars() {
    this.canv = $('#canv')[0]
    this.cttx = this.canv.getContext("2d")
    this.isMouseClicked = false
    this.isMouseInCanvas = false
    this.prevX = 0
    this.currX = 0
    this.prevY = 0
    this.currY = 0
  }

  initEvents() {
    $('#canv').on("mousemove", (e) => this.onMouseMove(e))
    $('#canv').on("mousedown", (e) => this.onMouseDown(e))
    $('#canv').on("mouseup", () => this.onMouseUp())
    $('#canv').on("mouseout", () => this.onMouseOut())
    $('#canv').on("mouseenter", (e) => this.onMouseEnter(e))
  }
  
  onMouseDown(e) {
  	this.isMouseClicked = true
    this.updateCurrentPosition(e)
  }
  
  onMouseUp() {
  	this.isMouseClicked = false
  }
  
  onMouseEnter(e) {
  	this.isMouseInCanvas = true
    this.updateCurrentPosition(e)
  }
  
  onMouseOut() {
  	this.isMouseInCanvas = false
  }

  onMouseMove(e) {
    if (this.isMouseClicked && this.isMouseInCanvas) {
    	this.updateCurrentPosition(e)
      this.draw()
    }
  }
  
  updateCurrentPosition(e) {
      this.prevX = this.currX
      this.prevY = this.currY
      this.currX = e.clientX - this.canv.offsetLeft
      this.currY = e.clientY - this.canv.offsetTop
  }
  
  draw() {
    this.cttx.beginPath()
    this.cttx.moveTo(this.prevX, this.prevY)
    this.cttx.lineTo(this.currX, this.currY)
    this.cttx.strokeStyle = "red"
    this.cttx.lineWidth = 5
    this.cttx.stroke()
    this.cttx.closePath()
  }
}

var canv = new SignTool()
document.body.appendChild(canv);

//////////////////////////////////////////////////////////////////////////////////////////const left = document.querySelectorAll("ul li");
const right = document.querySelectorAll(".right-icons ul li");
const dropzone = document.getElementById("dropzone");
const input = document.getElementById("input");
const search = document.getElementById("src")
const cross = document.getElementById("cls")
const find = document.getElementById("find")
const ser = document.getElementById("ser")
const group = document.getElementById("grp")
const slide = document.getElementById("slide")
const seek = document.getElementById("url")
const urlclose = document.getElementById("pop");
const musicclose = document.getElementById("popp");
const secclose = document.getElementById("poop");
const media = window.matchMedia("(max-width: 1100px)");
////////////////////////////////////////////////////////////////////////////////////////

if(media.matches) {
    document.getElementById("canv").style.left = "14.5rem"
    document.getElementById("canv").style.top = "8.8rem"
}




////////////////////////////////////////////////////////////////////////////////////////

document.getElementById("container").style.display = "none"
document.getElementById("canv").style.display = "none"
document.getElementById("songslist").style.opacity = 0;
document.getElementById("slide").style.opacity = 0;
document.getElementById("seconds").style.opacity = 0;
document.getElementById("ser").style.opacity = 0;
document.getElementById("demo").style.transform = "translateX(41rem) translateY(1rem)"
document.getElementById("demo").style.opacity = 0;
document.getElementById("demo").style.zIndex = -1;
document.getElementById("demo").style.fontFamily = "'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif";

//////////////////////////////////////////////////////////////////////////////////////
// document.getElementById("canvas").style.display = "none"

function mycrop() {
    if(document.getElementById("canv").style.display != "none") {
        document.getElementById("canv").style.display = "none"
    }
    if(img.style.display != "none") {
        document.getElementById("container").style.display = ""
    }else {
        document.getElementById("container").style.display = "none"
    }
}

//////////////////////////////////////////////////////////////////////////////////////

function mypen() {
    if(document.getElementById("container").style.display != "none") {
        document.getElementById("container").style.display = "none"
    }
    const btn = document.getElementById("btn")
    document.getElementById("canv").style.display = ""
    document.getElementById("canv").style.cursor = "pointer"
    btn.style.transform = "translateX(35rem) translateY(1.5rem)"
    document.getElementById("canvas").style.display = "none"

}

//////////////////////////////////////////////////////////////////////////////////////

function mytext() {
    if(document.getElementById("canv").style.display != "none") {
        document.getElementById("canv").style.display = "none"
    }
    if(document.getElementById("container").style.display != "none") {
        document.getElementById("container").style.display = "none"
    }
    if(document.getElementById("canvas").style.display != "none" || texxt.style.backgroundColor != "rgb(255, 255, 255)") {
        document.getElementById("canvas").style.display = "none"
        texxt.style.backgroundColor = "rgb(255, 255, 255)"
        }
        else {
            texxt.style.backgroundColor = "rgb(228, 228, 228, 0.5)"
        }
}

document.querySelector(".first").animate([
    {transform: "rotate(0)"},
    {transform: "rotate(360deg)"}
],{
    duration: 1000,
    iterations: Infinity
});
document.querySelector(".sec").animate([
    {transform: "rotate(0)"},
    {transform: "rotate(360deg)"}
],{
    duration: 1000,
    iterations: Infinity
});
document.querySelector(".thi").animate([
    {transform: "rotate(0)"},
    {transform: "rotate(360deg)"}
],{
    duration: 1000,
    iterations: Infinity
});
document.querySelector(".for").animate([
    {transform: "rotate(0)"},
    {transform: "rotate(360deg)"}
],{
    duration: 1000,
    iterations: Infinity
});
document.querySelector(".fiv").animate([
    {transform: "rotate(0)"},
    {transform: "rotate(360deg)"}
],{
    duration: 1000,
    iterations: Infinity
});
document.querySelector(".six").animate([
    {transform: "rotate(0)"},
    {transform: "rotate(360deg)"}
],{
    duration: 1000,
    iterations: Infinity
});
document.getElementById("f").animate([
    {transform: "rotate(0)"},
    {transform: "rotate(-360deg)"}
],{
    duration: 1000,
    iterations: Infinity
});
document.getElementById("s").animate([
    {transform: "rotate(0)"},
    {transform: "rotate(-360deg)"}
],{
    duration: 1000,
    iterations: Infinity
});
document.getElementById("t").animate([
    {transform: "rotate(0)"},
    {transform: "rotate(-360deg)"}
],{
    duration: 1000,
    iterations: Infinity
});
document.getElementById("fo").animate([
    {transform: "rotate(0)"},
    {transform: "rotate(-360deg)"}
],{
    duration: 1000,
    iterations: Infinity
});
document.getElementById("fi").animate([
    {transform: "rotate(0)"},
    {transform: "rotate(-360deg)"}
],{
    duration: 1000,
    iterations: Infinity
});
document.getElementById("si").animate([
    {transform: "rotate(0)"},
    {transform: "rotate(-360deg)"}
],{
    duration: 1000,
    iterations: Infinity
});

document.getElementById("fs").animate([
    {transform: "rotate(0)"},
    {transform: "rotate(360deg)"}
],{
    duration: 1000,
    iterations: Infinity
});
document.getElementById("se").animate([
    {transform: "rotate(0)"},
    {transform: "rotate(360deg)"}
],{
    duration: 1000,
    iterations: Infinity
});
document.getElementById("th").animate([
    {transform: "rotate(0)"},
    {transform: "rotate(360deg)"}
],{
    duration: 1000,
    iterations: Infinity
});
document.getElementById("fr").animate([
    {transform: "rotate(0)"},
    {transform: "rotate(360deg)"}
],{
    duration: 1000,
    iterations: Infinity
});
document.getElementById("fv").animate([
    {transform: "rotate(0)"},
    {transform: "rotate(360deg)"}
],{
    duration: 1000,
    iterations: Infinity
});
document.getElementById("sx").animate([
    {transform: "rotate(0)"},
    {transform: "rotate(360deg)"}
],{
    duration: 1000,
    iterations: Infinity
});


//////////////////////////////////////////////////////////////////////////////////////////


document.getElementById("seconds").addEventListener("mouseenter", ()=> {
    document.getElementById("infi").style.backgroundColor = "rgb(255, 255, 255)"
});

document.getElementById("slide").addEventListener("mouseenter", ()=> {
    document.getElementById("link").style.backgroundColor = "rgb(255, 255, 255)"
});

document.getElementById("songslist").addEventListener("mouseenter", ()=> {
    document.getElementById("music").style.backgroundColor = "rgb(255, 255, 255)"
});

document.getElementById("ser").addEventListener("mouseenter", ()=> {
    document.getElementById("find").style.backgroundColor = "rgb(255, 255, 255)"
});
//////////////////////////////////////////////////////////////////////////////////////////////
secclose.addEventListener("click", ()=> {
    document.getElementById("seconds").style.opacity = 0;
    document.getElementById("seconds").style.transform = "translateX(-200rem)"
});

secclose.addEventListener("mouseenter", ()=> {
    document.getElementById("infi").style.backgroundColor = "black"
});

document.getElementById("infi").addEventListener("mouseenter", ()=> {
    document.getElementById("infi").style.backgroundColor = "rgb(228, 228, 228, 0.5)"
});

document.getElementById("infi").addEventListener("mouseleave", ()=> {
    document.getElementById("infi").style.backgroundColor = "transparent"
});

document.getElementById("no0").addEventListener("click", ()=> {
    document.getElementById("barr").style.transform = "translateY(0rem)"
    document.getElementById("barr").style.transition = ".5s"
});
document.getElementById("no1").addEventListener("click", ()=> {
    document.getElementById("barr").style.transform = "translateY(23.2rem)"
    document.getElementById("barr").style.transition = ".5s"
});
document.getElementById("no2").addEventListener("click", ()=> {
    document.getElementById("barr").style.transform = "translateY(46.3rem)"
    document.getElementById("barr").style.transition = ".5s"
});
document.getElementById("no3").addEventListener("click", ()=> {
    document.getElementById("barr").style.transform = "translateY(69.4rem)"
    document.getElementById("barr").style.transition = ".5s"
});
document.getElementById("no4").addEventListener("click", ()=> {
    document.getElementById("barr").style.transform = "translateY(92.5rem)"
    document.getElementById("barr").style.transition = ".5s"
});
document.getElementById("no5").addEventListener("click", ()=> {
    document.getElementById("barr").style.transform = "translateY(115.6rem)"
    document.getElementById("barr").style.transition = ".5s"
});
document.getElementById("iff").addEventListener("click", ()=> {
    document.getElementById("barr").style.transform = "translateY(138.8rem)"
    document.getElementById("barr").style.transition = ".5s"
});


////////////////////////////////////////////////////////////////////////////////////////////////////////////////


document.getElementById("infi").addEventListener("click", ()=> {
    document.getElementById("seconds").style.opacity = 1;
    document.getElementById("seconds").style.transform = "translateX(0)"
    document.getElementById("seconds").style.transition = "0.5s"
});


document.getElementById("music").addEventListener("click", ()=> {
    document.getElementById("songslist").style.opacity = 1;
    document.getElementById("songslist").style.transform = "translateX(0)"
    document.getElementById("songslist").style.transition = ".5s"
    document.getElementById("songslist").style.backgroundColor = "rgb(251, 156, 118,0.9)"
});

musicclose.addEventListener("click", ()=> {
    document.getElementById("songslist").style.transform = "translateX(90rem)"
    document.getElementById("songslist").style.backgroundColor = "rgb(251, 156, 118,0.5)"
    document.getElementById("songslist").style.opacity = 0;
});

urlclose.addEventListener("mouseenter", ()=> {
    document.getElementById("link").style.backgroundColor = "transparent"
});

musicclose.addEventListener("mouseenter", ()=> {
  document.getElementById("music").style.backgroundColor = "transparent"
});

urlclose.addEventListener("click", ()=> {
    document.getElementById("slide").style.opacity = 0;
    slide.style.transform = "translateX(-90rem)";
    slide.style.backgroundColor = "rgba(162, 188, 236, 0.5)"
    slide.style.transition = ".5s"
});

  document.getElementById("link").addEventListener("click", ()=> {
    document.getElementById("slide").style.opacity = 1;
    slide.style.transform = "translateX(0rem)";
    slide.style.backgroundColor = "rgba(162, 200, 200, 0.9)"
    slide.style.transition = ".5s"
});


 document.getElementById("right").style.transform = "translateX(10rem)"
 document.getElementById("left").style.transform = "translateX(-10rem)"

seek.addEventListener("mouseenter", ()=> {
    seek.style.width = "26rem"
    seek.style.transition = ".5s"
});

seek.addEventListener("mouseleave", ()=> {
    seek.style.width = "25rem"
    seek.style.transition = ".5s"
});

input.addEventListener("click", ()=> {
    input.style.width = "60rem"
});


document.getElementById("ser").style.transform = "translateY(42rem)"
document.getElementById("ser").style.opacity = 0;


document.getElementById("find").addEventListener("click", ()=> {
    document.getElementById("ser").style.transform = "translateY(0rem)"
    document.getElementById("ser").style.transition = ".5s"
    document.getElementById("ser").style.opacity = 0.9;
    document.getElementById("find").style.backgroundColor = "rgb(255, 255, 255)"
});

document.getElementById("find").addEventListener("mouseenter", ()=> {
    document.getElementById("find").style.backgroundColor = "rgb(228, 228, 228, 0.5)"
});

document.getElementById("find").addEventListener("mouseleave", ()=> {
    document.getElementById("find").style.backgroundColor = "transparent"
});

document.getElementById("music").addEventListener("mouseenter", ()=> {
    document.getElementById("music").style.backgroundColor = "rgb(228, 228, 228, 0.5)"
});

document.getElementById("music").addEventListener("mouseleave", ()=> {
    document.getElementById("music").style.backgroundColor = "transparent"
});

document.getElementById("link").addEventListener("mouseenter", ()=> {
    document.getElementById("link").style.backgroundColor = "rgb(228, 228, 228, 0.5)"
});

document.getElementById("link").addEventListener("mouseleave", ()=> {
    document.getElementById("link").style.backgroundColor = "transparent"
});

document.getElementById("cls").addEventListener("click", ()=> {
    document.getElementById("ser").style.transform = "translateY(42rem)"
    document.getElementById("ser").style.opacity = 0;
    input.style.width = "30rem"
});

cross.addEventListener("mouseenter", ()=> {
    cross.style.opacity = 0.6;
    cross.style.border = "3px solid red"
    cross.style.transition = "300ms"
    document.getElementById("find").style.backgroundColor = "transparent"
});

cross.addEventListener("mouseleave", ()=> {
    cross.style.opacity = 1;
    cross.style.border = "3px solid white"
});

search.addEventListener("mouseenter", ()=> {
    search.style.boxShadow = "0 0 10px 0 white"
    search.style.opacity = 0.8;
    search.style.transition = "300ms"
});

search.addEventListener("mouseleave", ()=> {
    search.style.boxShadow = ""
    search.style.opacity = 1;
});

input.addEventListener("mouseenter", ()=> {
    input.style.border = "5px solid violet"
    input.style.transition = "300ms"
});
input.addEventListener("mouseleave", ()=> {
    input.style.border = ""
});

// Optional.   Show the copy icon when dragging over.  Seems to only work for chrome.
dropzone.addEventListener("dragover", function(e) {
    e.stopPropagation();
    e.preventDefault();
    e.dataTransfer.dropEffect = 'copy';
    dropzone.style.backgroundColor = "rgb(105, 151, 238, 0.2)";
});

// Get file data on drop
dropzone.addEventListener("drop", function(e) {
    const texxt = document.getElementById("text");
    const add = document.querySelector(".box i");
    const text = document.getElementById("h1")
    const close = document.querySelector(".close");
    e.stopPropagation();
    e.preventDefault();
    var files = e.dataTransfer.files; // Array of all files

    for(var i=0, file; file=files[i]; i++) {
        if(file.type.match(/image.*/)) {
            var reader = new FileReader();


            reader.onload = function(e) {

            // finished reading file data  
                var img = document.getElementById("img");

                texxt.addEventListener("click", ()=> {
                    img.style.cursor = "text"
                });
    
                document.getElementById("text").style.transform = "translateX(-10rem)"
                document.getElementById("pen").style.transform = "translateX(-10rem)"
                document.getElementById("music").style.transform = "translateX(-10rem)"
                document.getElementById("crop").style.transform = "translateX(-10rem)"

                document.getElementById("cut").style.transform = "translateX(10rem)"
                document.getElementById("find").style.transform = "translateX(10rem)"
                document.getElementById("link").style.transform = "translateX(10rem)"
                document.getElementById("infi").style.transform = "translateX(10rem)"
               
                dropzone.style.border = "0"
                img.style.display = "block"
                add.style.display = "none";
                text.style.display = "none";
                img.style.boxShadow = "0 0 8px 0 whitesmoke"
                dropzone.style.backgroundColor = "";
                img.src = e.target.result;
                dropzone.appendChild(img);
                close.addEventListener("click",() => {
                    img.style.display = "none";
                    add.style.display = "block";
                    text.style.display = "block"
                    dropzone.style.border = "3px dotted rgb(255, 255, 255, 0.5)"
                    document.getElementById("btn").style.transform = "translateX(35rem) translateY(-2.5rem)"
                    document.getElementById("container").style.display = "none"
                    document.getElementById("canv").style.display = "none"
                    document.getElementById("text").style.transform = "translateX(10rem)"
                    document.getElementById("pen").style.transform = "translateX(10rem)"
                    document.getElementById("music").style.transform = "translateX(10rem)"
                    document.getElementById("crop").style.transform = "translateX(10rem)"
    
                    document.getElementById("cut").style.transform = "translateX(-10rem)"
                    document.getElementById("find").style.transform = "translateX(-10rem)"
                    document.getElementById("link").style.transform = "translateX(-10rem)"
                    document.getElementById("infi").style.transform = "translateX(-10rem)"
                    close.style.transform = "translateY(-2rem) translateX(-50%)";
                    document.getElementById("canvas").style.display = "none";
                    document.getElementById("canv").style.display = "none"
                    img.style.boxShadow = "0 0 8px 0 whitesmoke"


        });

        }
            reader.readAsDataURL(file);  // finished reading file data.
            close.style.transform = "translateY(3.5rem) translateX(-50%)";
            close.style.transition = "0.5s"
            close.addEventListener("mouseenter", ()=> {
                var text = "close"
                document.getElementById("demo").style.color = "red"
                document.getElementById("demo").style.fontSize = "1.5rem"
                document.getElementById("demo").style.transition = ".5s"
                document.getElementById("demo").style.opacity = 1;
                document.getElementById("demo").style.transform = "translateX(44rem) translateY(1rem)"
                document.getElementById("demo").style.position = "absolute"
                document.getElementById("demo").innerHTML = text;
            });
                close.addEventListener("mouseleave", ()=> {
                    var text = "close"
                    document.getElementById("demo").style.color = "red"
                    document.getElementById("demo").style.fontSize = "1.5rem"
                    document.getElementById("demo").style.transition = ".5s"
                    document.getElementById("demo").style.opacity = 0;
                    document.getElementById("demo").style.transform = "translateX(41rem) translateY(1rem)"
                    document.getElementById("demo").style.position = "absolute"
                    document.getElementById("demo").innerHTML = text;
            });
            
        }
    
    }
});


 Array.from(left).forEach(items => {
    items.addEventListener("click", () => {
        var selected = document.getElementsByClassName("mystyle");
        selected[0].className = selected[0].className.replace(" mystyle", "");
        items.className += " mystyle";
        // items.classList.toggle('mystyle')  
    });
});

           
</script>
<script src="snap.js"></script>
</html>
