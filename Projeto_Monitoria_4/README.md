# Monitoria_Projeto_4

# Projeto 4 - Quem Poupa Tem

O novo banco QuemPoupaTem vai iniciar a sua operação em breve, mas não tem um sistema bancário estabelecido. Para desenvolver o sistema que controla os clientes, o banco decidiu contratar você.

O seu programa deve ser todo desenvolvido em C e pode ser feito até em trios.

## Requisitos
O banco trabalha com dois tipos de conta:
  1. Comum:
     * Cobra taxa de 5% a cada débito realizado
     * Permite um saldo negativo de até (R$ 1.000,00)
  3. Plus:
     * Cobra taxa de 3% a cada débito realizado
     * Permite um saldo negativo de até (R$ 5.000,00)

O sistema criado por você deve funcionar em loop infinito até que se deseje sair;

Um menu de opções deve ser sempre apresentado ao operador, contendo as seguintes operações:

1. Novo cliente
2. Apaga cliente
3. Listar clientes
4. Débito
5. Depósito
6. Extrato
7. Transferência Entre Contas
0. Sair

Cada opção deve ser implementada como uma função;
O seu programa deve conseguir armazenar até 1000 clientes e as informações das últimas 100 operações (depósito, saque, transferência) realizada pelo cliente
**IMPORTANTE:** Não se esqueça de que o banco não pode perder as informações se o programa terminar, fechar, parar de funcionar, ou o computador desligar. Todos os dados devem ser salvos de maneira permanente utilizando arquivos binários.

## Funções
- Opção 1 - Usada para criar novos clientes
  - Dados solicitados 
    - Nome
    - CPF
    - Tipo de conta (são dois: comum e plus)
    - Valor inicial da conta
    - Senha do usuário
---
- Opção 2 - Apaga o cliente pelo CPF
---
- Opção 3 - Listar todos os clientes
---
- Opção 4 - Serve para debitar um valor da conta do cliente
  - Dados solicitados: 
    - CPF
    - Senha
    - Valor
  - O débito somente pode ser feito se o CPF e a senha estiverem corretos.
---
- Opção 5 - Deposita um valor na conta do cliente
  - Dados solicitados:
    - CPF
    - Valor
---
- Opção 6 - Extrato - gera um arquivo com o histórico de todas as operações realizadas na conta, com valores, incluindo as tarifas.
  - Dados solicitados
    - CPF
    - Senha
  - O formato do extrato é livre, porém o arquivo de saída deve ser em formato txt e que possa ser aberto em qualquer editor de texto.
  - Não é necessário armazenar as datas das transações
  - O extrato só pode ser exibido se o CPF e senha estiverem corretos
---   
- Opção 7 - Transferência - realiza a transferência de uma valor determinado de uma conta (Origem) para outra conta (Destino)
  - Dados solicitados:
    - CPF (Origem)
    - Senha (Origem)
    - CPF (Destino)
    - Valor
  - O transferência só pode ser realizada se o CPF e a senha da conta de origem estiverem corretos

## Critérios de avaliação:
1. Implementação das funcionalidades (2 pontos):
    - a pontuação total será dividida entre todas as funcionalidades (7 itens acima + salvar e carregar o arquivo binário), além do tratamento de erro com mensagens avisando o usuário do que aconteceu durante a execução do programa e receberá nota máxima se funcionar
    - será apenas considerado o que está na branch principal do repositório (main ou master) e não serão considerados funcionalidades em outras branches
2. Uso correto do sistema de versionamento (3 pontos):
    - Uso do GitHub Workflow com issues e branches para cada funcionalidade do projeto (1.25 ponto)
    - Commits com partes que do projeto que funcionam (1.25 ponto)
    - README.md contendo descrição do projeto, como compilar e executar (0.5 ponto)
3. Desenvolvimento do código (5 pontos)
    - A correção do código será feita pelo que foi implementado em cada branch. Projetos sem branches receberão zero nesta parte
    - Cada funcionalidade é implementada em uma função
    - As funções não utilizam variáveis globais, a não ser que seja a única forma de resolver o problema
    - As funcionalidades implementadas seguem o que foi pedido
    - Variáveis declaradas com nomes que podem ser entendidos
    - Código que pode ser facilmente estendido
    - Sem loops, desvios condicionais, funções e variáveis desnecessárias
    - Tratamento de erros que podem ocorrer durante a execução do programa
    - Uso de tipos corretos para dados
    - Tratamento correto dos dados inseridos pelo usuário

## Critérios para zerar o projeto:
  - Plágio ou cópia mesmo que parcial
  - Programa que não compila/executa no replit
  - Entrega sem o uso de sistema de versionamento ou de outra forma (arquivo zip ou link para replit)
  - Upload de todo o código direto no repositório
  - Entrega apenas do binário, sem o código
  - Apenas receberão notas os participantes do projeto que tiverem commits que foram feito merge na branch main/master. Integrantes que não tiverem commits que tiveram merge na main não receberão nota
  - O projeto possui commits realizados após o horário final da entrega do projeto
