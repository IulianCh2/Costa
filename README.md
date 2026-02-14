
<html>
<head>
  <title>Oieiingat</title>
  <style>
    body {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background: pink;
      font-family: 'Comic Sans MS', sans-serif;
      text-align: center;
      overflow: hidden;
    }

    h1 {
      color: red;
      margin-bottom: 30px;
    }

    button {
      font-size: 18px;
      padding: 10px 20px;
      margin: 10px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      transition: all 0.3s ease;
    }

    #yes {
      background-color: #ff4d6d;
      color: white;
      position: relative;
      z-index: 1;
    }

    #no {
      background-color: white;
      color: #ff4d6d;
      border: 2px solid #ff4d6d;
      position: relative;
      z-index: 2;
    }
  </style>
</head>
<body>

  <h1>O iei in Gat ❤️</h1>

  <div>
    <button id="yes">Yes</button>
    <button id="no">No</button>
  </div>

  <script>
    const yesBtn = document.getElementById("yes");
    const noBtn = document.getElementById("no");

    let yesSize = 18;
    let noSize = 18;

    noBtn.onclick = function() {

      // Micșorăm NO
      noSize -= 2;
      if (noSize < 5) noSize = 5;

      noBtn.style.fontSize = noSize + "px";
      noBtn.style.padding = (noSize/2) + "px " + noSize + "px";

      // Mărim YES
      yesSize += 8;
      yesBtn.style.fontSize = yesSize + "px";
      yesBtn.style.padding = (yesSize/2) + "px " + yesSize + "px";

      // Când YES devine foarte mare
      if (yesSize > 120) {
        yesBtn.style.position = "fixed";
        yesBtn.style.top = "0";
        yesBtn.style.left = "0";
        yesBtn.style.width = "100vw";
        yesBtn.style.height = "100vh";
        yesBtn.style.fontSize = "50px";
        yesBtn.innerText = "YOU HAVE NO CHOICE 😈";
      }
    };

    yesBtn.onclick = function() {
      alert("Stiam eu ca vrei! 💕");
    };
  </script>

</body>
</html>
