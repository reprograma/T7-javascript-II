# Desafio

Faça um script que, usando apenas um laço for, exiba as duas colunas a seguir:

![](https://1.bp.blogspot.com/-8GN1llSTRjU/XA3E_BIfEQI/AAAAAAAAUpg/Nexl3gtxtq0JKrtT6F05M17tjdziI_GcgCLcBGAs/s1600/laco-for-javascript-loop.png)

# Questão resolvida e Código Comentado
Na figura temos duas coisas:
um valor que sobe de 0 até 10
um valor que cai de 10 até 0

O grande pulo do gato desse exercício é usar duas variáveis: a e b

A variável a inicia do 0 e vai sendo incrementada até chegar em 10.
Ao passo que b inicia de 10 e vai sendo decrementada em uma unidade até chegar a 0.

Na inicialização, criamos as duas variáveis e inicializamos ela corretamente.
Depois, temos dois testes: a deve ser menor ou igual a 10, e b deve ser maior ou igual a 0.
Por fim, demos um incremento (a++) e um decremento (b--).

Agora, dentro do laço FOR, é só imprimir linha por linha.
Primeiro o valor de a, depois um traço, o valor de b e uma quebra de linha do HTML (<br />)

# Código HTML + JavaScript

```
<!DOCTYPE html>
<html>
 <head>
   <title>Apostila JavaScript Progressivo</title>
   <script type="text/javascript" src="script.js"> </script>
 </head>
 <body>
    <script>exibir();</script>
 </body>
</html>
script.js
function exibir(){
  for(let a=0,  b=10 ; a<=10 &&  b>=0; a++, b--)
   document.write(a+" - "+b+"<br />");
}
```


