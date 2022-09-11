# Histórico de ver sões

| Versão  | Data     | Autor       | Descrição                   |
|---------|----------|-------------|-----------------------------|
| 0.1     |16/08/2022| @IanoMaciel | Estrutura inicial e Construção do tópico desenvolvimento do tópico **Introdutório** |
| 0.2     |17/08/2022| @IanoMaciel | Construção do tópico **Esquemático da Arquitetura** |
| 0.3     |18/08/2022| @IanoMaciel | Construção do subtópico **Tecnologias** |
| 0.4     |11/09/2022/ | @IanoMaciel | Contrução do tópico de Metas e Restrições da Arquitetura |
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

O MVC é um padrão de arquitetura de software, onde separa sua aplicação em três camadas, sendo elas *model*, *view* e *controller*. 

Nesse projeto a camada de interação do usuário (*View*), é a que faz a exibição dos dados, sendo o [React](https://pt-br.reactjs.org/docs/getting-started.html) e [React Native](https://reactnative.dev/docs/getting-started). Ambas tecnologias são bibliotecas do JavaScript, onde são responsável pela visualização web e mobile, respectivamente.

O *Model* é camada de manipulação dos dados, está camada é responsável pela leitura e escrita dos dados, neste caso foi utilizado o banco de dados [MongoDB Community Server](https://www.mongodb.com/try/download/community).

A camada de *Controller* funciona como intermediário, ou seja, coordenar o envio de requisições feitas entre a visão e o modelo. Para isso, será o utilizado o [NodeJs](https://nodejs.org/en/).

## Tecnologias 
| Tecnologias  | Descrição |
|--------------|-----------|
| React        | biblioteca do JavaScript para criação de interfaces de usuário em páginas web. | 
| React Native | é uma biblioteca Javascript criada pelo Facebook. É usada para desenvolver aplicativos para os sistemas Android e iOS de forma nativa. |
| Expo         | é uma estrutura/plataforma para aplicações universais react. É um conjunto de ferramentas e serviços construídos em torno de plataformas nativas (react native) que ajudam você a desenvolver, construir, implantar e rapidamente iterar em aplicativos iOS, Android e web a partir da mesma base de código JavaScript/TypeScript. |
| NodeJs       | Node.js é um software de código aberto, multiplataforma, baseado no interpretador V8 do Google e que permite a execução de códigos JavaScript fora de um navegador web. |
| Node Version Management | é uma ferramenta utilizada para versionamento do NodeJs |
| JavaScript   | Em conjunto com o HTML e CSS para o desenvolvimento front |
| MongoDB Community Server | é um software de banco de dados orientado a documentos livre, de código aberto e multiplataforma, escrito na linguagem C++. Classificado como um programa de banco de dados NoSQL, o MongoDB usa documentos semelhantes a JSON com esquemas. |

# Metas e Restrições da Arquitetura 
## Metas 
- Facilitar no gerenciamento de tarefas;
- Gerenciar tarefas do dia a dia dos usuários;
## Retrições 
- Ter acesso à internet

# Visão dos dados
## MER 
### Entidades 

USUÁRIO
| Atributos | Propriedades | Tipo | Descrição |
|-----------|--------------|------|-----------|
| macaddress | Chave obrigatória | String | ID do usuário |

# Caso de Uso 
![UC_ToDo](https://user-images.githubusercontent.com/71051791/185547903-6f9db7b3-ddac-491c-b9c5-bee3e7c3b427.png)

# Referências Bibliográficas
[Artefato: Documento de Arquitetura de Software](https://www.cin.ufpe.br/~gta/rup-vc/core.base_rup/workproducts/rup_software_architecture_document_C367485C.html)