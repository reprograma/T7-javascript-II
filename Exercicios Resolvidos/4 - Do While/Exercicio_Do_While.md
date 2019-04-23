# Desafio

Laços do while são muito usados para exibir menu, pedir dados, senhas...
Vamos criar um script que pede uma senha ao usuário.

Se a senha estiver correta, ele entra no sistema.
Se estiver errada, avisa e pede a senha novamente.

# Questão resolvida e Código Comentado
Funciona assim: ao clicar no botão Entrar, invocamos a função entrar() do JavaScript.

A senha digitada vai ser armazenada na variável senha.
Aí vamos pro do.

Lá nele, usando um prompt, pedimos a senha pro usuário.
Se ela for 2112js, aparece a mensagem de entrada no sistema.

Se não for, de senha inválida.

Isso vai acontecer indefinidamente, até o usuário digitar a senha corretamente, pois o teste condicional é: senha != '2112js'

Em outras palavras, isso quer dizer: 'usuário, enquanto a senha digitada não for a correta, vou ficar pedindo e testando, pedindo e testando...só paro quando digitar a senha correta.'

Leia em inglês: do ... while
Ou seja: faça, execute esse código, enquanto isso for verdade.

Note uma coisa importante: ele executa o código pelo menos uma vez!
Isso não acontece no laço WHILE.

Pro código rodar em WHILE, primeiro o teste tem que ser verdadeiro, senão nem entra.

# Código HTML + JavaScript



