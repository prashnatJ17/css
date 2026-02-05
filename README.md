<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>CSS Position Playground</title>
<style>
  body {
    height: 1500px; /* to show fixed box effect while scrolling */
    padding: 40px;
    font-family: Arial, sans-serif;
  }

  .container {
    position: relative;
    width: 500px;
    height: 300px;
    border: 2px dashed black;
    margin-top: 50px;
  }

  .box {
    width: 120px;
    height: 80px;
    color: white;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: bold;
  }

  /* Box 1 - static */
  .box1 {
    position: static;
    background-color: red;
  }

  /* Box 2 - relative */
  .box2 {
    position: relative;
    top: 20px;
    left: 40px;
    background-color: blue;
    z-index: 2; /* overlap effect */
  }

  /* Box 3 - absolute */
  .box3 {
    position: absolute;
    bottom: 10px;
    right: 10px;
    background-color: green;
    z-index: 1;
  }

  /* Box 4 - fixed */
  .box4 {
    position: fixed;
    bottom: 20px;
    right: 20px;
    background-color: purple;
  }
</style>
</head>
<body>

<h2>CSS Position Playground</h2>

<div class="container">
  <div class="box box1">Static</div>
  <div class="box box2">Relative</div>
  <div class="box box3">Absolute</div>
</div>

<div class="box box4">Fixed</div>

</body>
</html>



<!DOCTYPE html>
<html>
<head>
<title>Assignment 2</title>
<style>
body{
  margin:0;
  font-family: Arial, sans-serif;
}

.hero{
  height: 100vh;
  background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)),
  url("https://images.unsplash.com/photo-1501785888041-af3ef285b470") center/cover no-repeat;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  color: white;
}

.hero h1{
  font-size: 48px;
}

.hero p{
  margin: 10px 0 20px;
  font-size: 18px;
}

.btn{
  padding: 10px 20px;
  border-radius: 20px;
  border: 2px solid white;
  background: transparent;
  color: white;
  margin: 5px;
  cursor: pointer;
}

.btn.primary{
  background: teal;
  border-color: teal;
}
</style>
</head>
<body>

<div class="hero">
  <div>
    <h1>With Great Design<br>Comes Great Response</h1>
    <p>Make a beautiful website just the way you want it.</p>
    <button class="btn">Learn More</button>
    <button class="btn primary">Get Started</button>
  </div>
</div>

</body>
</html>






<!DOCTYPE html>
<html>
<head>
<title>Assignment 3</title>
<style>
body{
  background: #ffe0b2;
  font-family: Arial, sans-serif;
  display:flex;
  justify-content:center;
  align-items:center;
  height:100vh;
}

.card{
  width: 800px;
  height: 350px;
  background: white;
  border-radius: 20px;
  display:flex;
  justify-content: space-between;
  align-items:center;
  padding: 40px;
  box-shadow: 0 20px 40px rgba(0,0,0,0.2);
}

.text h1{
  font-size: 36px;
}

.text button{
  margin-top: 15px;
  padding: 10px 20px;
  border:none;
  background: orange;
  color:white;
  border-radius: 8px;
  cursor:pointer;
}

.img img{
  height: 300px;
}
</style>
</head>
<body>

<div class="card">
  <div class="text">
    <h1>It’s time to stand out<br>from the crowd.</h1>
    <button>New Collection</button>
  </div>
  <div class="img">
    <img src="c:\Users\tejas\Downloads\fashion-pretty-cool-youngwith-shopping-bags-wearing-black-hat-white-pants-over-colorful-orange-background-79063329.webp" alt="model">
  </div>
</div>

</body>
</html>







<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Discover The World</title>
<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family: Arial, sans-serif;
}

body{
    background:#0b0b0b;
    display:flex;
    justify-content:center;
    align-items:center;
    height:100vh;
}

/* Main Card */
.container{
    width:900px;
    background:#ffffff;
    border-radius:16px;
    padding:40px;
    display:flex;
    align-items:center;
    gap:40px;
    box-shadow:0 20px 40px rgba(0,0,0,0.3);
}

/* Left Content */
.left h1{
    font-size:42px;
    line-height:1.1;
}

.left h1 span{
    color:#1e73be;
    font-style:italic;
}

.left p{
    margin:15px 0 25px;
    color:#666;
    font-size:14px;
}

/* Buttons */
.buttons{
    display:flex;
    gap:15px;
}

.btn{
    padding:10px 20px;
    border-radius:25px;
    border:none;
    cursor:pointer;
    font-size:14px;
}

.btn-primary{
    background:#1e73be;
    color:white;
}

.btn-secondary{
    background:#eef4fb;
    color:#1e73be;
}

/* Stats Boxes */
.stats{
    display:flex;
    gap:15px;
    margin-top:30px;
}

.stat-box{
    background:#1e73be;
    color:white;
    padding:12px 18px;
    border-radius:10px;
    font-size:13px;
    text-align:center;
}

/* Right Image Section */
.right{
    position:relative;
}

.bg-shape{
    width:300px;
    height:200px;
    background:#1e73be;
    border-radius:20px;
}

.traveler{
    position:absolute;
    top:-40px;
    left:60px;
    width:200px;
}
</style>
</head>
<body>

<div class="container">

    <!-- Left Section -->
    <div class="left">
        <h1><span>Discover</span><br>The World</h1>
        <p>
            Let's embark on a global journey, immersing ourselves in diverse cultures 
            and creating unforgettable memories as we travel the world.
        </p>

        <div class="buttons">
            <button class="btn btn-primary">Explore More</button>
            <button class="btn btn-secondary">Watch Demo</button>
        </div>

        <div class="stats">
            <div class="stat-box">64+<br>Countries</div>
            <div class="stat-box">24M+<br>Per Year User</div>
            <div class="stat-box">03k+<br>Experiences</div>
        </div>
    </div>

    <!-- Right Section -->
    <div class="right">
        <div class="bg-shape"></div>
        <img class="traveler" src="https://images.unsplash.com/photo-1521737604893-d14cc237f11d?w=400" alt="Traveler">
    </div>

</div>

</body>
</html>
