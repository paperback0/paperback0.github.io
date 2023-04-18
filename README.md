# paperback0.github.io
<!DOCTYPE html>
<html>
<head>
  <title>Text Encoder/Decoder</title>
  <style>
    label {
      display: block;
      margin-top: 10px;
    }
    input[type="text"] {
      width: 90%;
      padding: 5px;
      font-size: 16px;
    }
    button {
      padding: 5px 10px;
      font-size: 16px;
      margin-top: 10px;
    }
    #output2, #output4 {
      margin-top: 10px;
      border: 1px solid #ccc;
      padding: 5px;
      font-size: 16px;
    }
  </style>
</head>
<body>
  <h1>Text Encoder / Decoder</h1>
  <label for="input1">Input:</label>
  <input type="text" id="input1">
  <button onclick="encode()">Encode</button><br>
  <br>
  <label for="output2">Output:</label>
  <input type="text" id="output2" readonly><br>
  <br>
  <label for="input3">Input:</label>
  <input type="text" id="input3">
  <button onclick="decode()">Decode</button><br>
  <br>
  <label for="output4">Output:</label>
  <input type="text" id="output4" readonly>
  <script>
    function encode() {
      const input1 = document.getElementById('input1');
      const output2 = document.getElementById('output2');
      output2.value = btoa(input1.value);
    }
    function decode() {
      const input3 = document.getElementById('input3');
      const output4 = document.getElementById('output4');
      output4.value = atob(input3.value);
    }
  </script>
</body>
</html>

