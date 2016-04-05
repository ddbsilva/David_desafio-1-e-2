# David_desafio-1-e-2

#David Diego de Brito / Email: ddbsilva@gmail.com
# Desafio 1:  Dado um numero inteiro N positivo e uma sequencia com N numeros inteiros, determinar o maior e o menor número da sequencia.

<html>
<head><title></title></head>
<body>

<SCRIPT LANGUAGE="JavaScript" TYPE="text/javascript">

var vetor = new Array ();
var i, proximo;

nunInt = parseInt (prompt("Digite um número inteiro : ", ""));

for (i = 0; i < nunInt; i++) {
proximo = vetor.length;

vetor[proximo] = parseInt (prompt("Digite um número inteiro : ", ""));

}
var menor = Math.min.apply(null, vetor );
var maior = Math.max.apply(null, vetor );
document.write('<h2>Maior número = '+maior + "<br>" + 'Menor número = '+menor +'</h2>');


</SCRIPT>
</SCRIPT>
</body>
</html>

#####################################################################################################################

#David Diego de Brito / Email: ddbsilva@gmail.com
#Desafio 2: Calculadora simples PHP 


<!DOCTYPE HTML>
<html lang = "pt-br">
<head>
   <title>Calculadora</title>
   <meta charset = "UTF-8">
</head>
<body>
			<h1>CALCULADORA</h1>
   <form action="" method="post" >
   <label for="nome">Primeiro Numero:</label>
      <input type="text" name="val1"><br>
	  
	  <label for="nome">Operador:</label>
	  <input type="radio" name="operador" value="+">
	  <label for="+">+</label>
      <input type="radio" name="operador" value="-">
	  <label for="-">-</label>
      <input type="radio" name="operador" value="*">
	  <label for="*">*</label>
      <input type="radio" name="operador" value="/">
	  <label for="/">/</label><br>
	  <label for="nome">Segundo numero:</label>	  
      <input type="text" name="val2"><br>
      
	  <input type="submit" value="Calcular">
   </form> 

</body>
</html>
<?php  
   if( !empty($_POST["val2"]) ) {
      if($_POST["operador"] == '+')
         $calc = $_POST["val1"] + $_POST["val2"];
      else if($_POST["operador"] == '-')
         $calc = $_POST["val1"] -$_POST["val2"];
      else if($_POST["operador"] == '*')
         $calc = $_POST["num1"]*$_POST["val2"];
      else
         $calc = $_POST["val1"]/$_POST["val2"];

      echo "<h2>O resultado é: $calc</h2>";
   }
?>       
