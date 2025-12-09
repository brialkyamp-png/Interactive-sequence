<!DOCTYPE html>
<html>
<head>
  <title>Interactive Quiz</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      margin-top: 50px;
      background-color: #f0f0f0;
    }
    .container {
      max-width: 500px;
      margin: auto;
      padding: 30px;
      border: 2px solid #333;
      border-radius: 12px;
      background-color: #fff;
    }
    button {
      margin: 10px;
      padding: 12px 25px;
      font-size: 16px;
      cursor: pointer;
    }
  </style>
  <script>
    function step1() {
      document.getElementById("message").innerText = "Your name is: Deusdedit Nyamwamu";
      document.getElementById("correctBtn").style.display = "inline-block";
      document.getElementById("wrongBtn").style.display = "inline-block";
      
      document.getElementById("correctBtn").onclick = step2;
      document.getElementById("wrongBtn").onclick = wrongStep;
    }

    function step2() {
      document.getElementById("message").innerText = "You studied at St Charles Lwanga School, Kitui";
      document.getElementById("correctBtn").onclick = step3;
      document.getElementById("wrongBtn").onclick = wrongStep;
    }

    function step3() {
      document.getElementById("message").innerText = "THIS PROGRAM IS CREATED BY BRIAN KYAMBIA THE COMPUTER MASTER 😂😂😂😂";
      document.getElementById("correctBtn").style.display = "none";
      document.getElementById("wrongBtn").style.display = "none";
    }

    function wrongStep() {
      document.getElementById("message").innerText = "YOU ARE VERY STUPID 😜";
      document.getElementById("correctBtn").style.display = "none";
      document.getElementById("wrongBtn").style.display = "none";
    }

    window.onload = step1;
  </script>
</head>
<body>
  <div class="container">
    <h2 id="message"></h2>
    <button id="correctBtn">Correct</button>
    <button id="wrongBtn">Wrong</button>
  </div>
</body>
</html>


---

