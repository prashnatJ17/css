# css
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
