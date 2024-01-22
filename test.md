<!DOCTYPE html>
<html>
  <head>
    <title>String Replacement</title>
    <style>
      .container {
        margin: 20px;
      }
      label {
        font-weight: bold;
      }
      input {
        margin-bottom: 10px;
      }
    </style>
  </head>
  <body>
    <div class="container">
      <h1>String Replacement</h1>
      <label for="originalString">Original String:</label>
      <input type="text" id="originalString" /><br />
      <label for="replacementWord">Replacement Word:</label>
      <input type="text" id="replacementWord" /><br />
      <button onclick="replaceWord()">Replace</button>
      <p id="output"></p>
    </div>

    <script>
      function replaceWord() {
        var originalString = document.getElementById("originalString").value;
        var replacementWord = document.getElementById("replacementWord").value;
        var newString = originalString.replace("user", replacementWord);
        document.getElementById("output").textContent = newString;
      }
    </script>
  </body>
</html>
