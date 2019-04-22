# Desafio

Escreva uma página que pede ao usuário um número de 1 até 12, e mostra o mês correspondente a este número. Por exemplo, 1 é Janeiro, 2 é Fevereiro etc.

# Questão resolvida e Código Comentado
Exibimos um formulário, de id=numero, do tipo numérico e pedimos o número para o usuário.
Em seguida, um botão chama a função exibir() do JavaScript, ao ser acionado (clicado).

Vamos para o JS.
Pegamos o que foi digitado no campo numero pelo usuário, passamos para inteiro (parseInt) e armazenamos na variável mes, dentro de nosso código JavaScript.

Depois, jogamos essa variável no switch.
E fazemos:
case 1: alert("Janeiro")
case 2: alert("Fevereiro")
etc

Ou seja, se o mes digitado for 1, vai aparecer uma janela dizendo que o mês é Janeiro.
Se o usuário tiver digitado 2, a janela vai mostrar Fevereiro, e assim sucessivamente.

# Código HTML + JavaScript

```
<!DOCTYPE html>
<html>
 <head>
   <title>Curso JavaScript Progressivo</title>
   Digite um mês de 1 até 12:<input id="numero" type="number"> <br />
   <button onclick="exibir()">Exibir mês</button>

   <script type="text/javascript">

    function exibir(){
     var mes = parseInt(document.getElementById("numero").value);
     
     switch(mes){
      case 1:  alert("Janeiro");
      case 2:  alert("Fevereiro");
      case 3:  alert("Março");
      case 4:  alert("Abril");
      case 5:  alert("Maio");
      case 6:  alert("Junho");
      case 7:  alert("Julho");
      case 8:  alert("Agosto");
      case 9:  alert("Setembro");
      case 10: alert("Outubro");
      case 11: alert("Novembro");
      case 12: alert("Dezembro");
     }
    }
 </script>

 </head>
</html>
```


