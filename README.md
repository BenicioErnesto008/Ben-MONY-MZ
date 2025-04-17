<!DOCTYPE html><html lang="pt">
<head>
  <meta charset="UTF-8">
  <title>BEM MONY MZ</title>
  <style>
    body {
      background-color: black;
      color: lime;
      font-family: monospace;
      padding: 20px;
    }
    .container {
      max-width: 500px;
      margin: auto;
    }
    input, button, select {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      background-color: #111;
      color: lime;
      border: 1px solid lime;
    }
    .plan {
      border: 1px solid lime;
      padding: 10px;
      margin-top: 10px;
      cursor: pointer;
    }
    .hidden {
      display: none;
    }
  </style>
  <script>
    function mostrarCodigo(valor) {
      document.getElementById('codigoContainer').classList.remove('hidden');
      document.getElementById('valorSelecionado').value = valor;
    }
  </script>
</head>
<body>
  <div class="container">
    <h1>BEM MONY MZ</h1>
    <p>Cadastre-se para começar a investir:</p>
    <input type="text" placeholder="Nome completo">
    <input type="text" placeholder="Número de telefone">
    <input type="email" placeholder="Email">
    <input type="password" placeholder="Palavra-passe"><h2>Escolha o valor de investimento</h2>
<div class="plan" onclick="mostrarCodigo('50=100 (500MT Real)')">50MT = 100MT</div>
<div class="plan" onclick="mostrarCodigo('500=500')">500MT = 500MT</div>
<div class="plan" onclick="mostrarCodigo('1000=1000')">1000MT = 1000MT</div>
<div class="plan" onclick="mostrarCodigo('1500=2500')">1500MT = 2500MT</div>
<div class="plan" onclick="mostrarCodigo('2000=5000')">2000MT = 5000MT</div>

<div id="codigoContainer" class="hidden">
  <h3>Insira o código de envio via M-Pesa ou e-Mola</h3>
  <input type="text" placeholder="Código de transação">
  <input type="hidden" id="valorSelecionado">
  <button>Confirmar Investimento</button>
</div>

<p style="margin-top: 30px; font-size: 12px;">Validade do site até: 16/04/2026</p>

  </div>
</body>
</html
