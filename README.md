!DOCTYPE html>
<html>
<head>
  <title>Interactive Sequence</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      margin-top: 50px;
    }
    .container {
      max-width: 400px;
      margin: auto;
      padding: 20px;
      border: 2px solid #333;
      border-radius: 10px;
      background-color: #f0f0f0;
    }
    button {
      margin: 10px;
      padding: 10px 20px;
      font-size: 16px;
      cursor: pointer;
    }
  </style>
  <script>
    function step1() {
      document.getElementById("message").innerText = "Your names are: Deusdedit Nyamwamu";
      document.getElementById("nextBtn").style.display = "inline-block";
      document.getElementById("cancelBtn").style.display = "inline-block";
      document.getElementById("nextBtn").onclick = step2;
      document.getElementById("cancelBtn").onclick = stopSequence;
    }

    function step2() {
      document.getElementById("message").innerText = "You studied in St Charles Lwanga School, Kitui";
      document.getElementById("nextBtn").onclick = step3;
      document.getElementById("cancelBtn").onclick = stopSequence;
    }

    function step3() {
      document.getElementById("message").innerText = "This information has been carefully created by BRIAN KYAMBIA to Mkisiiii 😂😂😂😂";
      document.getElementById("nextBtn").style.display = "none";
      document.getElementById("cancelBtn").style.display = "none";
    }

    function stopSequence() {
      document.getElementById("message").innerText = "Sequence stopped.";
      document.getElementById("nextBtn").style.display = "none";
      document.getElementById("cancelBtn").style.display = "none";
    }

    window.onload = step1;
  </script>
</head>
<body>
  <div class="container">
    <h2 id="message"></h2>
    <button id="nextBtn">Next</button>
    <button id="cancelBtn">Cancel</button>
  </div>
</body>
</html># Interactive-sequence
