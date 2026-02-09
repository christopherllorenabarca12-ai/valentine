<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Be My Valentine 💖</title>

<style>
  body {
    margin: 0;
    height: 100vh;
    background-image: url("https://drive.google.com/file/d/1m1-TyvbTmzroJgeuO3lYY6RM_TgwdBch/view?usp=drive_link");
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    display: flex;
    justify-content: center;
    align-items: center;
    font-family: Arial, sans-serif;
  }

  .overlay {
    background: rgba(0, 0, 0, 0.55);
    padding: 40px;
    border-radius: 20px;
    text-align: center;
    color: white;
    position: relative;
  }

  h1 {
    margin-bottom: 30px;
  }

  button {
    padding: 12px 28px;
    font-size: 18px;
    border: none;
    border-radius: 30px;
    cursor: pointer;
    margin: 10px;
  }

  #yes {
    background-color: #ff4d6d;
    color: white;
  }

  #no {
    background-color: #ccc;
    color: black;
    position: absolute;
  }
</style>
</head>

<body>

<div class="overlay">
  <h1>💖 Will you be my Valentine? 💖</h1>
  <button id="yes">YES 💌</button>
  <button id="no">NO 🙈</button>
</div>

<script>
  const noBtn = document.getElementById("no");

  noBtn.addEventListener("mouseover", () => {
    const x = Math.random() * (window.innerWidth - 100);
    const y = Math.random() * (window.innerHeight - 50);
    noBtn.style.left = x + "px";
    noBtn.style.top = y + "px";
  });

  document.getElementById("yes").addEventListener("click", () => {
    window.location.href =
      "mailto:christopherllorenabarca12@gmail.com" +
      "?subject=Valentine%20Date%20Accepted%20💖" +
      "&body=Yes!%20I%20would%20love%20to%20be%20your%20Valentine%20🥰💐";
  });
</script>

</body>
</html>
