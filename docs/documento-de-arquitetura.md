
# PDF2K-Nativo
***
# Documento de Arquitetura

***
## Histórico de Revisão
***
| Data | Versão | Descrição | Autor |
|:----:|:------:|:---------:|:-----:|
| 03/09/18 | 0.1 | Abertura do Documento de Arquitetura | Brian Lui |
| 03/09/18 | 0.2 | Metas e Restrições de Arquitetura | Brian Lui |
| 03/09/18 | 0.3 | Representação da Arquitetura | Rafael Teodosio |
| 06/09/18 | 0.4 | Arquitetura de serviços e referenciais | Wictor Girardi |
| 07/09/18 | 0.5 | Introdução | Julio Litwin |
| 07/09/18 | 0.6 | Visão geral | Wictor Girardi |
| 12/09/18 | 0.7 | Diagrama de Casos de Uso| Luís Cláudio T. Lima
|18/09/18 | 0.8 | Revisão da Representação da Arquitetura | Rafael Teodosio
|24/09/18 | 1.0 | Revisão Geral | Rafael Teodosio
|22/11/18 | 1.1 | Revisão de Documento | Wictor Girardi
|24/11/18 | 1.2 | Revisão de Documento | Wictor Girardi
***
### 1. Introdução
***

#### 1.1 Finalidade

Este documento apresenta uma visão geral da arquitetura do sistema e utiliza uma série de visões arquiteturais diferentes para ilustrar os diversos aspectos do sistema. Sua intenção é capturar e transmitir as decisões significativas do ponto de vista da arquitetura que foram tomadas em relação ao sistema.

#### 1.2 Escopo

O PDF2CASH é um software projetado para processamento de PDF’s nativos, focado em diferentes tipos de notas fiscais eletrônicas. Possibilitando assim a análise simples e automatizada de notas fiscais eletrônicas e seu armazenamento de forma segura em nosso programa, dentre outras features.

Neste documento, será tratado todas as informações de arquitetura do software, como diagramas de classes, casos de testes, casos de uso e dentre outros.

#### 1.3 Definições, Acrônimos e Abreviações

>MVT(Model View template): Arquitetura de software utilizada em sistemas que desejam separar a modelagem de dados, interface e processamento de requisições em camadas independentes.

>Active View: Biblioteca do framework ruby, responsável por implementar o tratamento de requisições da view.

>Active Controller: Biblioteca do framework ruby que implementa toda a camada Controller.

>Active Record: Biblioteca do framework ruby on rails que implementa
operações da camada Model.

>JSON(JavaScript Object Notation): Formato de texto com uma formatação leve de troca de dados.


#### 1.4 Referências
> BORGES, Ateldy; MATIAS, Bruno; Rodrigues, Carlos Enrique; MARQUES, Daniel; COUTINHO, Francisco Wallacy; SANTOS, Yasmin; DADAMOS, Rodrigo. **SIGS**: Documento de Arquitetura. Disponível em:
https://github.com/fga-eps-mds/2017.1-SIGS/wiki/Documento-de-Arquitetura

***

***
### 2. Representação da Arquitetura

A arquitetura utilizada contém dois ambientes diferentes para a nossa aplicação, o ambiente de controle de dados que é conhecido como API e o um ambiente web desenvolvido em ReactJS para os usuários, contemplando um sistema onde usuários podem criar seus projetos, importar dados e adicionar colaboradores.

Com relação a API, o projeto PDF2CA$H será desenvolvido utilizando o framework Django com a API REST.
A API REST é um estilo de arquitetura para fornecer padrões entre sistemas de computador na Web, facilitando a comunicação entre os sistemas. São caracterizados pela forma como são sem estado e separam as preocupações do cliente e do servidor.

Dentro do framework Django Rest existem:

* **Serializers** : Os Serializers permitem que dados complexos, como querysets e instâncias de modelos, sejam convertidos em tipos de dados Python nativos que podem ser facilmente renderizados em JSON, ou outros tipos de conteúdo.

* **End Points**: Um Endpoint de um serviço Web é a URL onde seu serviço pode ser acessado por uma aplicação cliente.

* **View Set**: Uma classe view set é uma classe baseada da views do Django, não possuindo assim metodos como .get(), .post() e outros.

A parte visual da aplicação será feita em ReactJS, React é uma biblioteca JavaScript declarativa, eficiente e flexível para a criação de interfaces de usuário (UI) criada pelo Facebook.

A arquitetura será representada da seguinte forma:

![Dcu3](img/dcuuu.png)

* **SQLite**: Banco de dados utilizado por nossa aplicação que armazena notas fiscais e funcionarios.  

* **PDFToInvoice**: É uma aplicação que utiliza a tecnologia Django Rest que trata as informações obtidas pelo parser e as direciona de maneira filtrada para o FrontEnd. Sendo um dos tratamentos que o PDFToInvoice é responsável é realizar a filtração das informações a serem passadas para o frontEnd para serem realizadas a geração de gráficos. Alem disso, ele recebe os dados do FrontEnd e os armazena no banco de dados SQLite.

* **API Gateway**: API Gateway é o único ponto de entrada para todos os clientes manipulando todas as solicitações, permitindo a criação, controle, edição e visualização de usuários e de administradores que utilizarão a aplicação e realizarão requisições. Realizando todos esses processos de maneira autenticada e segura, limitando o acesso a determinadas partes do programa de acordo com o grau de poder que o cliente possui.

* **CloudUpdater**: É um microsserviço que recebe os builds dos outros repositórios existentes e tem a capacidade de servir-los ao launcher.

* **FrontEnd**: Utilizando tecnologias como React Next, esse microsserviço interage diretamente com o usuário, manda e recebe requisições do Django. Utiliza também um pacote do React Js que possibilita a criação de gráficos a partir dos dados obtidos pelo programa.

***

### 3. Metas e Restrições de Arquitetura

***

 O projeto PDF2CA$H possui as seguintes metas:

* Suporte com os principais navegadores web da atualidade : Google Chrome, Internet Explorer, Microsoft Edge e Mozilla Firefox.

* Suporte a diferentes sistemas operacionais como Windows, Linux e MacOs.

Logo abaixo será apresentada as restrições da arquitetura:
* Framework Django 2.0.3 com Python 3.5.2
* Django REST: um framework utilizada para construção de WEB APIs
* Banco de dados relacional SQLite


***
### 4. Visão Geral
***

#### 4.1 Atores

#### 4.2 Administrador

O administrador além de poder realizar todas as funcionalidades que o usuário comum é habilitado, ele ainda pode manter funcionários, que significa a capacidade de criar, editar, visualizar e deletar funcionários cadastrados.

O Administrador é uma peça chave na execução do programa, para a criação de usuários e cadastramento de notas fiscais é necessários que haja um administrador cadastrado e logado no sistema, possuindo assim a maior permissão dentro do programa, criando, editando e deletando os funcionários cadastrados por si mesmo e suas notas ficais.

#### 4.3 Usuário

O Usuário comum pode visualizar a empresa da qual está cadastrado, adicionar notas fiscais ao programa, gerenciar as análises baseadas nas notas fiscais geradas pelo programa assim como visualizar, modificar e deletar as notas fiscais já existentes.

#### 4.4 Diagrama de Casos de Uso         
![Dcuv2](img/dcuv2.jpg)

#### 4.4.1 Versões anteriores
* [Diagrama de caso de uso V-8](img/ducv3.jpg)
* [Diagrama de caso de uso V-7](img/dcu-6.jpg)
* [Diagrama de caso de uso V-6](img/dcu-5.jpg)
* [Diagrama de caso de uso V-5](img/dcu-4.jpg)
* [Diagrama de caso de uso V-4](img/dcu-3.jpg)
* [Diagrama de caso de uso V-3](img/dcu-2.jpg)
* [Diagrama de caso de uso V-2](img/dcu-1.jpg)
* [Diagrama de caso de uso V-1](img/dcu.png)



#### 4.5 Descrição dos Casos de Uso

##### UC01 - Cadastrar Administrador:
Esse caso de uso permite que o usuário se cadastre como administrador e assim poder manter os usuários.
##### UC02 - Efetuar Login:
Esse caso de uso permite que o usuário consiga usar as funcionalidades do sistema.
##### UC03 - Adicionar PDF de Nota Fiscal:
Esse caso de uso permite que o usuário adicione uma ou mais notas fiscais no sistema.
##### UC04 - Visualizar Análise:
Esse caso de uso permite ao usuário e ao administrador visualizar as análises das notas fiscais.
##### UC05 - Listar Notas Fiscais:
Esse caso de uso permite que o usuário listar todas as notas fiscais.
##### UC06 - Visualizar Nota Fiscal:
Esse caso de uso permite ao usuário visualizar os dados de alguma nota fiscal.
##### UC07 - Manter funcionarios:
Esse caso de uso permite que o administrador gerencie os outros usuarios, sendo possivel criar, deletar, modificar e visualizar.
##### UC08 - Remover Nota Fiscal:
Esse caso de uso permite ao usuário e ao administrador remover um ou mais notas fiscais.

***
### 5. Arquitetura dos Serviços e Visão de Implementação
***

#### 5.1 Visão Geral


#### 5.1.1. Model
As Models do MVT e do MV são equivalentes em responsabilidades. O framework Django facilita na interface com o banco de dados. Cada classe da modelo se compara a uma tabela do banco de dados, e as instâncias destas classes, representam os registros destas tabelas. Para adicionar valores ao banco, basta defini-los nas respectivas variáveis. Esta camada contém qualquer coisa e tudo sobre os dados: como acessá-lo , como validá-lo , quais comportamentos que têm e as relações entre os dados. Para o mapeamento dos dados, não será necessário utilizar códigos em SQL para garantir a persistência dos dados no banco.

#### 5.1.2. View
A camada View é responsável pela implementação das regras de apresentação e negócio do nosso sistema. É nela onde iremos nos comunicar com a Model, cadastrando e tratando as informações recebidas. Retornando para o usuário uma resposta, como HTMLs, XML, ou erros encontrados.

#### 5.1.3. Detalhes arquiteturais de projetos Django
As resoluções de urls, responsabilidade dada às controllers no MVT(que no nosso caso do Django Rest é MV), é feita pela própria estrutura do framework;
O Django oferece uma interface com o banco de dados que permite ao desenvolvedor não se preocupar com a conexão entre suas classes de domínio e banco.

#### 5.2 ReactJs

O React.JS é uma biblioteca JavaScript do Facebook para construir interfaces de usuário, não se tratando assim de um framework. Diferentemente do Backbone.JS, AngularJS, Ember e outros que fornecem todos os componentes necessários para uma aplicação front-end, o React se preocupa apenas com a parte de view,
isso quer dizer que ele não assume nada em relação ao seu stack e não fornece nenhuma camada de service, controller, model, collection, routes e etc.
O React trabalha apenas com o conceito de componente que recebe propriedades, computa o estado e retorna uma representação virtual do DOM,
isso quer dizer que componentes do React não trabalham com templates propriamente ditas, como Handlebars.js ou Hogan.js, a forma como ele lida com isso é estruturando a representação do HTML em objetos.

#### 5.2.1 Electron

O Electron foi desenvolvido para permitir que o desenvolvimento de aplicações desktop usando JavaScript, HTML e CSS fosse muito mais fácil. Criado pela equipe do GitHub, ficou conhecido no começo como Atom Shell. O Electron foi criado usando tecnologias como o Node.js e o Chromium, e atualmente roda em ambiente de produção de vários projetos, como o próprio editor Atom e outros, como o Slack e o Visual Studio Code. Ele é um framework bem simples de trabalhar e de rápida configuração, para construção de pequenas e grandes aplicações desktop.

Ao ser executado, um aplicativo Electron mínimo é composto de pelo menos dois processos: o processo principal e um processo 'renderer'. Como são processos separados, eles executam scripts Javascript diferentes, em contextos diferentes (um não interfere no outro).
O processo principal é onde tudo começa. No aplicativo de exemplo, o script main.js roda no processo principal. O ambiente é muito semelhante ao Node.js "puro". Quando este processo cria um objeto BrowserWindow, aparece uma janela de UI. (A rigor um app Electron não precisa ter UI mas aí faria mais sentido rodá-lo diretamente no Node.js.)
Cada janela de UI é um browser, e para cada janela é criado um processo 'renderer'. O conteúdo da UI é construído com HTML5: abre-se uma página HTML com CSS e eventual código Javascript. O script renderer.js do exemplo roda no contexto do processo 'renderer'. No exemplo, ele não faz nada, mas além das APIs HTML5 ele também tem acesso às APIs do Node.js (e portanto às APIs do Electron).
Como são processos separados, é preciso usar uma API de IPC para trocar mensagens entre o processo principal e o(s) processo(s) 'renderer', se necessário.
Como é de se esperar, algumas tarefas só podem ser levadas a cabo pelo script do processo principal (exemplo: adicionar um ícone no 'tray' da barra de tarefas). Também haverá tarefas do seu aplicativo que talvez só façam sentido no processo principal.
O interpretador do script main.js não é o Node.js instalado em sua máquina; mas sim um binário do próprio Electron (que incorpora versões estáticas do Node.js e do Chromium). Isso elimina toda uma classe de problemas de dependências, e simplifica muito o empacotamento final da aplicação.


#### 5.3 Micro Serviços e Camadas
Microsserviços é uma abordagem que desenvolve um aplicativo único como uma suite de pequenos serviços, cada um executando seu próprio processo e se comunicando através de mecanismos leves, muitas vezes em uma API com recursos HTTP. Esses serviços são construídos em torno de capacidades de negócios e funcionam através de mecanismos de deploy independentes totalmente automatizados. Há o mínimo possível de gerenciamento centralizado desses serviços, que podem ser escritos em diferentes linguagens de programação e utilizam diferentes tecnologias de armazenamento de dados. Cada serviço é desenvolvido em torno de um conjunto de regras de negócio específico, e é implementado de forma independente.
Com isso, consegue-se quebrar algumas barreiras existentes no modelo de arquitetura monolítica:

#### 5.3.1 Manutenção e evolução dos serviços mais estáveis
Os desenvolvedores tratarão de códigos que executam uma única função, e cada serviço individual não cresce indefinidamente com o crescimento do sistema.
#### 5.3.2 Serviços com baixo nível de acoplamento e interdependência
Dessa forma, a manutenção em um serviço não interfere diretamente em outras funcionalidades do sistema.
#### 5.3.3 Escalabilidade do sistema
É obtida com o deploy e replicação de micro serviços através da infraestrutura de servidores, máquinas virtuais e containers de forma independente. Isso torna o crescimento e a possibilidade de adaptação do sistema muito mais flexível.
#### 5.3.4 Redução de custos
Como cada aplicação só utiliza os serviços de que necessita, os custos são diretamente associados à funcionalidade e à carga de uso do sistema, não sendo necessário carregar custos associados a funcionalidades não utilizadas.
#### 5.3.5 Flexibilidade de tecnologia
Não é necessário amarrar os desenvolvedores a uma tecnologia específica, pois há baixo acoplamento entre os serviços. Dessa forma, pode ser utilizada a melhor tecnologia para atender a cada caso, além da possibilidade de evoluir o sistema continuamente, diminuindo o risco da obsolescência tecnológica.
#### 5.3.6 Facilidade de colocar alterações em produção
As mudanças no sistema são feitas através das alterações e evoluções feitas nos serviços. Assim, não existe um sistema que precisa ser reinicializado para continuar funcionando. O time de desenvolvimento que precisará acompanhar a mudança será o time responsável pelos serviços que estão sendo alterados.


***
### 7. Referências
***
[Business Intelligence]
https://inteligencia.rockcontent.com/business-intelligence/

[What is REST]
https://www.codecademy.com/articles/what-is-rest

[Django REST Framework] http://www.django-rest-framework.org/api-guide/serializers

[Modelo MVT em Django]   
https://github.com/fga-eps-mds/A-Disciplina/wiki/Padr%C3%B5es-Arquiteturais---MVC-X-Arquitetura-do-Django

[Micro Serviços: Qual a diferença para arquitetura monolitica] https://www.opus-software.com.br/micro-servicos-arquietura-monolitica/
