# Planejamento: Sistema de Almoxarifado

## 1. Requisitos Funcionais
* [RF01] Cadastro de Itens: O sistema deve permitir registrar o nome e a marca de um produto novo.
* [RF02] Controle de Entrada e Saída: O usuário deve conseguir registrar quantas unidades de um produto estão entrando ou saindo do almoxarifado.
* [RF03] Consulta de Estoque: O sistema deve exibir uma lista clara com todos os produtos e a quantidade que temos disponível de cada um no momento.
* [RF04] Histórico: O usuário deve conseguir ver o histórico do que aconteceu com cada produto (ex: "hoje entraram 10 peças").

## 2. Requisitos Não Funcionais
* [RNF01] Responsividade: O sistema deve funcionar bem tanto em telas de computador quanto em celulares. Os botões de "Entrada" e "Saída" devem ser fáceis de clicar mesmo em telas pequenas (telas sensíveis ao toque).
* [RNF02] Simplicidade: A interface deve ser direta, evitando menus complicados para que o funcionário do almoxarifado consiga registrar uma movimentação em poucos segundos.
* [RNF03] Segurança: Garantir que apenas usuários autorizados possam alterar o estoque e cadastrar produtos.

## 3. Regras de Negócio
* [RN01] Consistência: O saldo do produto na tabela de "Produtos" deve ser sempre o resultado da soma de todas as entradas menos a soma de todas as saídas registradas na tabela de "Movimentações". 
* [RN02] Não permitir saldo negativo: O sistema não deve permitir que uma "Saída" seja registrada se não houver estoque suficiente, para evitar erros no almoxarifado.
* [RN03] Rastreabilidade: Toda movimentação deve registrar a data e o motivo (entrada ou saída) para podermos conferir o inventário futuramente.