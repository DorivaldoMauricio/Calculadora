# Calculadora
Calculadora básica feito com HTML
<!DOCTYPE html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Calculadora de gorjetas</title>
  </head>
 <body>
   <div id="container">
     <div>
     <h1 class="title">Calculadora de Gorjetas</h1>
     </div>
     <div>
       <form class="tipsform" id="tipsform">
         <label for="bill">
            <p>Quanto ficou a conta?</p>
          </label>       
         <p>
           KZ <input type="number" placeholder="100" name="bill" id="bill" class="formInput" required>
         </p>
         <label for="serviceQual">
            <p>Como foi seu serviço?</p>
         </label>
         <p>
           <select name="serviceQual" id="serviceQual" class="formSelect" required>
             <option disable selected value="0">-- Escolha uma opção </option>
             <option value="0.3">30% - Incrível</option>
             <option value="0.2">20% - Bom</option>
             <option value="0.15">15% - Aceitável</option>
             <option value="0.1">10% - Ruim</option>
             <option value="0.05">05% - Péssimo</option>
           </select>
         </p>
          <label for="people">        
           <p>Quantas pessoas vão dividir a conta?</p>
          </label>
         <p>
           <input type="number" placeholder="1" name="people" id="people" class="formInput" required> Pessoa(s)
         </p>
         <button type="submit" class="formSubmit">Calcular!</button>
       </form> 
     </div>
     <div id="totalTip">
      Gorjeta Total:
      KZ<span id="tip">0.00</span>
     <p id="each">Cada</p>
     </div>
   </div>
   <script type="text/javascript" src="Scripts.js"></script>
  </body>
</html>
