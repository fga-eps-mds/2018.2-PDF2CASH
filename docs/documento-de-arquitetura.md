
# PDF2K-Nativo

## Documento de Arquitetura

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


***
### 4. Visão Geral
***

#### 4.1 Atores

#### 4.2 Administrador

O Administrador pode manter usuários cadastrados, manter empresas cadastradas assim como remover, visualizar e editar notas fiscais.

#### 4.3 Usuário

O Usuário comum pode visualizar a empresa da qual está cadastrado, adicionar notas fiscais ao programa, gerenciar as análises baseadas nas notas fiscais geradas pelo programa assim como visualizar, modificar e deletar as notas fiscais já existentes.
4.2              Diagramas de caso de uso




#### 4.3 Descrição dos Casos de Uso

##### UC01 - (ME) Manter Empresa:
Esse caso de uso permite que o usuário com acesso de administrador no programa possui o poder de criar, manter, modificar ou deletar as empresas adicionadas por ele ao programa.
##### UC02 - Manter User:
Esse caso de uso permite que o administrador possui o poder de criar, deletar, modificar ou manter usuários em suas empresas cadastradas.
###### UC03 - (MA) Manter Analise:
Esse caso de uso permite que o usuário tenha o poder de criar, deletar, modificar ou manter análises baseadas nas notas fiscais existentes.
###### UC04 - (RNF) Remover Nota Fiscal:
Esse caso de uso permite ao usuário e ao administrador remover as notas fiscais já existentes no programa, de maneira completa ou não.
###### UC05 -(VE) Visualizar Empresa:
Esse caso de uso permite que o usuário visualizar a empresa da qual é cadastrado.
###### UC06 - (ANF) Adicionar Nota Fiscal:
Esse caso de uso permite ao usuário fazer a adição de notas fiscais ao programa.
###### UC07 -(ENF) Editar Nota Fiscal:
 Esse caso de uso permite ao usuário fazer a edição de uma nota fiscal.
###### UC08 -(VNF) Visualizar Nota Fiscal:
Esse caso de uso permite ao usuário e ao administrador visualizarem uma nota fiscal.


***
### 5. Arquitetura dos Serviços e Visão de Implementação
***

#### 5.1 Visão Geral

Modelo MVT:

#### 5.1.1. Model
As Models do MVC e do MVT são equivalentes em responsabilidades. O framework Django facilita na interface com o banco de dados. Cada classe da modelo se compara a uma tabela do banco de dados, e as instâncias destas classes, representam os registros destas tabelas. Para adicionar valores ao banco, basta defini-los nas respectivas variáveis. Esta camada contém qualquer coisa e tudo sobre os dados: como acessá-lo , como validá-lo , quais comportamentos que têm e as relações entre os dados. Para o mapeamento dos dados, não será necessário utilizar códigos em SQL para garantir a persistência dos dados no banco.

#### 5.1.2. View
A camada View é responsável pela implementação das regras de apresentação e negócio do nosso sistema. É nela onde iremos nos comunicar com a Model e a Template, cadastrando e tratando as informações recebidas. Retornando para o usuário uma resposta, como HTMLs, XML, ou erros encontrados.

#### 5.1.3. Template
Templates é a camada que retorna a visão para o usuário do programa. Essa camada é composta por, HTML,CSS, javascript e etc. Geralmente linguagens focadas na apresentação do site para o usuário.

#### 5.1.3. Detalhes arquiteturais de projetos Django
As resoluções de urls, responsabilidade dada às controllers no MVC, é feita pela própria estrutura do framework;
O Django oferece uma interface com o banco de dados que permite ao desenvolvedor não se preocupar com a conexão entre suas classes de domínio e banco.

#### 5.1.4. Electron
O Electron foi desenvolvido para permitir que o desenvolvimento de aplicações desktop usando JavaScript, HTML e CSS fosse muito mais fácil. Criado pela equipe do GitHub, ficou conhecido no começo como Atom Shell. O Electron foi criado usando tecnologias como o Node.js e o Chromium, e atualmente roda em ambiente de produção de vários projetos, como o próprio editor Atom e outros, como o Slack e o Visual Studio Code. Ele é um framework bem simples de trabalhar e de rápida configuração, para construção de pequenas e grandes aplicações desktop.

#### 5.1.5. Funcionamento Electron
Ao ser executado, um aplicativo Electron mínimo é composto de pelo menos dois processos: o processo principal e um processo 'renderer'. Como são processos separados, eles executam scripts Javascript diferentes, em contextos diferentes (um não interfere no outro).
O processo principal é onde tudo começa. No aplicativo de exemplo, o script main.js roda no processo principal. O ambiente é muito semelhante ao Node.js "puro". Quando este processo cria um objeto BrowserWindow, aparece uma janela de UI. (A rigor um app Electron não precisa ter UI mas aí faria mais sentido rodá-lo diretamente no Node.js.)
Cada janela de UI é um browser, e para cada janela é criado um processo 'renderer'. O conteúdo da UI é construído com HTML5: abre-se uma página HTML com CSS e eventual código Javascript. O script renderer.js do exemplo roda no contexto do processo 'renderer'. No exemplo, ele não faz nada, mas além das APIs HTML5 ele também tem acesso às APIs do Node.js (e portanto às APIs do Electron).
Como são processos separados, é preciso usar uma API de IPC para trocar mensagens entre o processo principal e o(s) processo(s) 'renderer', se necessário.
Como é de se esperar, algumas tarefas só podem ser levadas a cabo pelo script do processo principal (exemplo: adicionar um ícone no 'tray' da barra de tarefas). Também haverá tarefas do seu aplicativo que talvez só façam sentido no processo principal.
O interpretador do script main.js não é o Node.js instalado em sua máquina; mas sim um binário do próprio Electron (que incorpora versões estáticas do Node.js e do Chromium). Isso elimina toda uma classe de problemas de dependências, e simplifica muito o empacotamento final da aplicação.





#### 5.2 Micro Serviços e Camadas
A arquitetura de micro serviços é utilizada para desenvolver uma aplicação como um conjunto de pequenos serviços, cada um funcionando em seu próprio processo. Cada serviço é desenvolvido em torno de um conjunto de regras de negócio específico, e é implementado de forma independente.
Com isso, consegue-se quebrar algumas barreiras existentes no modelo de arquitetura monolítica:
#### 5.2.1 Manutenção e evolução dos serviços mais estáveis
Os desenvolvedores tratarão de códigos que executam uma única função, e cada serviço individual não cresce indefinidamente com o crescimento do sistema.
#### 5.2.2 Serviços com baixo nível de acoplamento e interdependência
Dessa forma, a manutenção em um serviço não interfere diretamente em outras funcionalidades do sistema.
#### 5.2.3 Escalabilidade do sistema
É obtida com o deploy e replicação de micro serviços através da infraestrutura de servidores, máquinas virtuais e containers de forma independente. Isso torna o crescimento e a possibilidade de adaptação do sistema muito mais flexível.
#### 5.2.4 Redução de custos
Como cada aplicação só utiliza os serviços de que necessita, os custos são diretamente associados à funcionalidade e à carga de uso do sistema, não sendo necessário carregar custos associados a funcionalidades não utilizadas.
#### 5.2.5 Flexibilidade de tecnologia
Não é necessário amarrar os desenvolvedores a uma tecnologia específica, pois há baixo acoplamento entre os serviços. Dessa forma, pode ser utilizada a melhor tecnologia para atender a cada caso, além da possibilidade de evoluir o sistema continuamente, diminuindo o risco da obsolescência tecnológica.
#### 5.2.6 Facilidade de colocar alterações em produção
As mudanças no sistema são feitas através das alterações e evoluções feitas nos serviços. Assim, não existe um sistema que precisa ser reinicializado para continuar funcionando. O time de desenvolvimento que precisará acompanhar a mudança será o time responsável pelos serviços que estão sendo alterados.
