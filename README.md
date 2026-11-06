# Caixa_eletronico
Simulador de Caixa Eletrônico
Este projeto é um simulador básico de caixa eletrônico (ATM) desenvolvido na linguagem C. Ele foi criado para praticar conceitos fundamentais de programação, como laços de repetição, estruturas de decisão e operações matemáticas simples.

O que o projeto faz
O sistema apresenta um menu interativo onde é possível realizar operações básicas de uma conta bancária:

Consulta de Saldo: Exibe o valor disponível na conta. O programa já inicia com um saldo predefinido de R$ 10.000 para facilitar a realização dos testes.

Saque de Dinheiro: Permite retirar um valor específico. O sistema verifica automaticamente se o valor é maior que zero, se há saldo suficiente e se é múltiplo de 5 (já que as notas disponíveis são de 100, 50, 20, 10 e 5). Sendo aprovado, ele calcula e exibe a menor quantidade de notas que serão entregues.

Sair: Encerra a aplicação de forma segura e interativa.

Entendendo o Código
A lógica do programa foi construída passo a passo utilizando recursos essenciais da linguagem C para criar uma navegação fluida:

Organização e Variáveis: O código começa separando os espaços na memória necessários para guardar o saldo, os valores digitados e as "caixinhas" para contar a quantidade de cada nota.

Menu Contínuo: Utiliza a estrutura de repetição do-while para manter o programa rodando. O menu sempre reaparece após uma operação, encerrando apenas quando a opção 3 é escolhida.

Navegação de Opções: A estrutura switch funciona como um painel de controle, guiando o programa para a ação correta dependendo do número que você digita.

Lógica do Saque: Usando condições if, o programa barra saques inválidos. A contagem das notas é feita usando matemática direta: ele divide o valor do saque por 100 para saber quantas notas de 100 entregar, e usa o resto dessa divisão (operador %) para calcular as notas seguintes, passando por 50, 20, 10, até chegar em 5.

Como testar o projeto
Para rodar este simulador, o processo é bem visual e não requer comandos complexos de terminal. Basta abrir o arquivo do código diretamente no Visual Studio Code, garantindo que você tenha a extensão e o compilador de C instalados. Ao executar, o menu interativo aparecerá na aba de saída ou no terminal integrado da própria ferramenta, aguardando a sua escolha e guiando o processo passo a passo.
