
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
      transition: transform 0.2s;
    }
    button:hover {
      transform: scale(1.1);
    }
    #yes {
      background-color: #ff4d6d;
      color: white;
    }
    #no {
      background-color: #fff;
      color: #ff4d6d;
      border: 2px solid #ff4d6d;
    }
  </style>
</head>
<body>
  <h1>You will be my Valentine ❤️</h1>
  <div>
    <button id="yes">Yes</button>
    <button id="no">No</button>
  </div>

  <script>
    document.getElementById('yes').onclick = function() {
      alert("Yay! 💖 I'm so happy! 💕");
    };
    document.getElementById('no').onclick = function() {
      alert("Oh no 😢 But you're still awesome!");
    };
  </script>
</body>
</html>
