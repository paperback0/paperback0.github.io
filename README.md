# paperback0.github.io
<!DOCTYPE html>
<html>
  <head>
    <title>Text Encryption and Decryption</title>
  </head>
  <body>
    <h1>Text Encryption and Decryption</h1>
    <label for="input-text">Input Text:</label>
    <input type="text" id="input-text" /><br /><br />
    <button onclick="encrypt()">Encrypt</button>
    <button onclick="decrypt()">Decrypt</button><br /><br />
    <label for="encrypted-text">Encrypted Text:</label>
    <input type="text" id="encrypted-text" /><br /><br />
    <label for="decrypted-text">Decrypted Text:</label>
    <input type="text" id="decrypted-text" /><br /><br />

    <script>
      function encrypt() {
        const inputText = document.getElementById("input-text").value;
        const encryptedText = btoa(inputText);
        document.getElementById("encrypted-text").value = encryptedText;
      }

      function decrypt() {
        const encryptedText = document.getElementById("encrypted-text").value;
        const decryptedText = atob(encryptedText);
        document.getElementById("decrypted-text").value = decryptedText;
      }
    </script>
  </body>
</html>
