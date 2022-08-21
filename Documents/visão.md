# Histórico de Versões
| Versão  | Data       | Autor       | Descrição                   |
|---------|------------|-------------|-----------------------------|
| 1.0     | 19/08/2022 | @IanoMaciel | Criação do documento de visão |
| 1.1     | 20/08/2022 | @IanoMaciel | Inserção dos requisitos funcionais e não funcionais | 
| 1.2     | 21/08/2022 | @IanoMaciel | Construção do Regra de Negócio | 

# 1. Introdução 
## 1.1 Propósito do Documento de Requisitos

Esse documento tem o objetivo de detalhar os requisitos dos usuários que deverão ser atendidos pelo aplicativo a ser construído nesse projeto. Ele servirá como base para a construção do sistema por parte dos programadores. Aqui estará presente uma descrição detalhada das funções do produto, de suas interfaces e do comportamento esperado do sistema.

## 1.2 Público Alvo

Este documento destina-se aos stackholders (arquitetos de software, engenheiros de software, testadores e usuários classificados como usuários fornecedores).

# 2. Descrição Geral do Produto
Um pouco sobre o projeto **ToDo**. É uma ferramenta que busca auxiliar os usuários com as tarefas cotidianas, com ele, será permitido que você agende uma nova tarefa além de notificar tarefas atrasadas. Além da aplicação web, ele contará com uma aplicação *mobile* onde será permitido a sincronização de atividades com o *smathphone* do usuário. 

## 2.2 Escopo

| Nº | Módulo | Descrição |
|----|--------|-----------|
| 1  | Aplicativo | Será desenvolvimento um sistema web para atendenter os sistemas operacionais Mac OS, Windows e Linux. |
| 2 | Aplicativo | Será desenvolvido um aplicativo *mobile* para atender os sistemas operacionais iOS e Android. | 

## 2.3 Atores 

| Nº | Ator | Definição e Privilégio de Acessso e Segurança |
|----|------|-----------------------------------------------|
| 1  | Usário | Será possível realizar todas as funções dos que o aplicativo irá fornecer. | 

# 3. Requisitos

## 3.1 Requisitos Funcionais

| ID | Descrição | Prioridade |
|----|-----------|------------|
| RF01 | O Sistema deve permitir ao usuário criar novas tarefas | Essencial |
| RF02 | O Sistema deve permitir ao usuário atualizar tarefa  | Essencial |
| RF03 | O Sistema deve permitir ao usuário excluir tarefas | Essencial |
| RF04 | O Sistema deve permitir ao usuário listar todas as informações | Essencial |
| RF05 | O Sistema deve permitir ao usuário listar tarefas do dia | Essencial |
| RF06 | O Sistema deve permitir ao usuário listar tarefas da semana | Essencial |
| RF07 | O Sistema deve permitir ao usuário listar tarefas do mês | Essencial |
| RF08 | O Sistema deve permitir ao usuário listar tarefas do Ano | Essencial |
| RF09 | O sistema deve permitir ao usuário listar tarefas atrasadas | Essencial |

## 3.2 Requisitos Não Funcionais

| ID | Descrição | Prioridade | 
|----|-----------|------------|
| RNF01 | Os dados serão gravados no MongoDb. | Segurança |
| RNF02 | O sistema será desenvolvido para web e mobile. | Interoperabilidade |
| RNF03 | O sistema deve utilizar a linguagem de progtamação JavaScript em conjunto como suas bibliotecas React e React Native e auxilio do Expo. | Portabilidade |
| RNF04 | O sistema deve dispor de design responsivo. | Usabilidade | 
| RNF05 | A interface em ambos sistemas será de fácil manipulação | Usabilidade | 
| RNF06 | O sistema deve utilizar o padrão UML 2.0 para a documentação. | Padrões |

# 4. Regras de Negócio

| Nº | Requisito Associado |  Nome do RN |  Descrição | 
|----|---------------------|-------------|------------|
| RN01 | RF01 | New task | O usuário poderá criar novas tarefas, para isso, será necessário informar os seguintes campos: tipo de tarefa, título, descrição, data e hora. | 
| RN01 | RF02 | Update | O usuário |

![UC_ToDo](https://user-images.githubusercontent.com/71051791/185547903-6f9db7b3-ddac-491c-b9c5-bee3e7c3b427.png)