<svelte:head>
    <title>Calc</title>
</svelte:head>
<div class="container">
    <h1>Calc</h1>

  <input type="text" id="num1" placeholder="Введите 1 число" class="input1">
  <input type="text" id="num2" placeholder="Введите 2 число" class="input2">
  <button onclick="add()" class="plus">+</button>
  <button onclick="subtract()" class="minus">-</button>
  <button onclick="multiply()" class="multiply">*</button>
  <button onclick="divide()" class="divide">/</button>

  <h2 id="result" class="result"> </h2>

<style>
    .container {
        margin: 50px auto;
        max-width: 800px;
        padding: 0 20px;
        background-color: rgb(186, 195, 253);
    }

    .input1 {
        border-style: dashed;
    }

    .input2 {
        border-style: dashed;
    }
</style>

  <script>
    function add() {
      const num1 = parseFloat(document.getElementById('num1').value);
      const num2 = parseFloat(document.getElementById('num2').value);
      document.getElementById('result').innerText = num1 + num2;
    }

    function subtract() {
      const num1 = parseFloat(document.getElementById('num1').value);
      const num2 = parseFloat(document.getElementById('num2').value);
      document.getElementById('result').innerText = num1 - num2;
    }

    function multiply() {
      const num1 = parseFloat(document.getElementById('num1').value);
      const num2 = parseFloat(document.getElementById('num2').value);
      document.getElementById('result').innerText = num1 * num2;
    }

    function divide() {
      const num1 = parseFloat(document.getElementById('num1').value);
      const num2 = parseFloat(document.getElementById('num2').value);
      document.getElementById('result').innerText = num1 / num2;
    }
  </script>
</div>
