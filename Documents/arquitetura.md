# Histório de versões

| Versão  | Data     | Autor       | Descrição                   |
|---------|----------|-------------|-----------------------------|
| 0.1     |16/08/2022| @IanoMaciel | Estrutura inicial e Construção do tópico desenvolvimento do tópico Introdutório           |

# Introdução 
## Objetivo 
Este documento tem a finalidade de fornecer uma visão arquitetural do Projeto **ToDo.** Além disso, conta com informações que irá auxiliar os desenvolvedores e gestores para compreender a arquitetura utilizada no desenvolvimento, fluxos de informações e as tenclogias envolvidas neste projeto. 
## Escopo
Um pouco sobre o projeto **ToDo**. É uma ferramenta que busca auxiliar os usuários com as tarefas cotidianas, com ele, será permitido que você agende uma nova tarefa além de notificar tarefas atrasadas. Além da aplicação web, ele contará com uma aplicação *mobile* onde será permitido a sincronização de atividades com o *smathphone* do usuário. 
## Visão Geral 
O documento está segmento em Representação de Arquitetura, Metas e Restrições da Arquitetura, Visão de Casos de Uso, Visão Lógica e Visão de Dados.
## Definições, Acrônimos  e Abreviações
- **API - Application Programming Interface:** é um conjunto de rotinas e padrões estabelecidos por um software para a utilização das suas funcionalidades por aplicativos que não pretendem envolver-se em detalhes da implementação do software, mas apenas usar seus serviços.
- **Framework**: é uma abstração que une códigos comuns entre vários projetos de software provendo uma funcionalidade genérica.
# Esquemático da Arquitetura
## Padrão Arquitetural 

![mvc_arquitetura](https://user-images.githubusercontent.com/71051791/184946453-46ad1447-d4a6-4df1-9f37-3d73f62a7a2a.png)
O MVC é um padrão de arquitetura de software, onde separa sua aplicação em três camadas, sendo elas model, view e controller. Nesse projeto a camada de interação do usuário (view), é a que faz a exibição dos dados, sendo ela por meio do framework react.js e next.js; a camada de manipulação dos dados (model), responsável pela leitura e escrita dos dados no banco de dados, nesse caso postgres usando a ferramenta sequelize, e também suas validações e a camada de controle (controller), responsável por receber todas as requisições do usuário, controlando qual model usar e qual view será mostrado ao usuário. Essa divisão em camadas é realizada para facilitar a resolução de um problema maior.





# Metas e Restrições da Arquitetura 

# Visão dos dados

# Caso de Uso 

# Referências Bibliográficas
[Artefato: Documento de Arquitetura de Software](https://www.cin.ufpe.br/~gta/rup-vc/core.base_rup/workproducts/rup_software_architecture_document_C367485C.html)