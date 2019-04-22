# Desafio

Faça um script que pede duas notas de um aluno. Em seguida ele deve calcular a média do aluno e dar o seguinte resultado:
 - A mensagem "Aprovado", se a média alcançada for maior ou igual a sete;
 - A mensagem "Reprovado", se a média for menor do que sete;
 - A mensagem "Aprovado com Distinção", se a média for igual a dez.

# Questão resolvida e Código Comentado
Inicialmente, criamos dois campos de input em HTML, do tipo number, para receber as notas dos alunos e um botão 'Calcular média', que quando acionado chama a função media(), que vai dentro do código JS.

Vamos lá, inicialmente, declaramos duas variáveis nota1 e a nota2, que vão receber os dados digitados nos formulários de input.

Como esses dados vem no formato string, precisamos transformar eles em dados números do tipo decimal, por isso usamos a função parseFloat().

Com os dois números em mãos, declaramos a variável media, que recebe o valor da média das duas notas (somamos elas e dividimos por 2).

Agora pegamos esse valor, e vamos usar nos testes condicionais.
Se este valor for maior ou igual a 7, é porque foi aprovado.

Mas temos dois tipos de aprovações.
Então, dentro do IF, testamos se essa nota é igual a 10. Se for, dizemos que foi aprovado com distinção. Se não for, é porque a nota é maior ou igual a 7 e é menor que 10, logo dizemos apenas que foi aprovado.

Se o primeiro IF for falso, é porque a nota é menor que 7, cai no ELSE com a mensagem de provação.

# Código HTML + JavaScript

```
<!DOCTYPE html>
<html>
 <head>

   <title>Exercicio If ... Else</title>

   Primeira nota <input id="nota1" type="number"> <br />
   Segunda  nota <input id="nota2" type="number"> <br />

   <button onclick="media()">Calcular Média</button>

   <script type="text/javascript">

    function media(){
     let nota1 = parseFloat(document.getElementById("nota1").value);
     let nota2 = parseFloat(document.getElementById("nota2").value);

     let media = (nota1 + nota2)/2 ;

     if(media >= 7)
      if(media==10)
       alert("Uau! Aprovado com distinção");
      else
       alert("Parabéns, aprovado! Media "+media);
     else
      alert("Reprovado!")

    }
 </script>

 </head>
</html>
```


