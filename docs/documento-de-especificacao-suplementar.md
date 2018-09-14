# PDF2Cash
***
# Especificação Suplementar
***

## 4. Confiabilidade
Um dos requisitos para o bom funcionamento do sistema, será um alto nível de confiabilidade. De tal modo que a probabilidade da ocorrência de erros, falhas e bugs em algum sistema operacional seja mínima e que sejam sanadas o mais rápido possível.
O PDF2CASH poderá ser operado 24H por dia para que a manutenção seja contínua, e assim os erros serem corrigidos rapidamente para que não gere transtornos a empresa.

## 5. Desempenho
Deverá ser uma aplicação leve para que seja possível o uso do mesmo nas mais diferentes configurações de computadores e, também, terá que possuir um tempo de resposta rápido e preciso tanto com a elaboração de gráficos com os dados já adquiridos quanto com os dados presentes na nota fiscal.

## 6. Portabilidade
Para o uso do sistema será necessário que os dispositivos tenham um dos Sistemas Operacionais seguintes: Windows, Linux e OS. Poderá ser realizado o Download do programa em um dos seguintes navegadores com acesso a internet : Google Chrome, Mozilla Firefox e Apple Safari.

7.                  Interoperabilidade
O PDF2CASH haverá conexão com banco de dados, utilizando-se o postgreSQL, onde será armazenado: dados de contas (administradores e usuários), as notas fiscais processadas pelo PDF2CASH, com as informações exigidas. Sendo assim, tendo o banco de dados como um centro de informações, podendo chamar/atualizar/processar dados remotamente.

8.                  Segurança
Os dados no PDF2CASH apenas serão processados a partir de um controle de usuário, sendo assim, será necessário logar-se e ter os devidos privilégios na conta de usuário (sendo distinguindo em administrador e usuário). Administrador terá o seu papel em adicionar/excluir/editar os próprios usuários, empresas e dentre outros, portanto, tendo todos os privilégios de um usuário, contudo, um usuário será quem irá gerenciar as notas fiscais, processar notas fiscais, adicionar, editar e excluir. Para mais informações, é possível obter em Documento de Arquitetura - Tópico: 4. Visão Geral. Buscando incluir boas práticas de segurança de informações, como segurança das operações e comunicações, controle de acesso e dentre outros.

## 9. Restrições de Design
O PDF2CASH será uma aplicação minimalista e com cores que não tragam cansaço para a vista do usuário. As informações, links e botões serão organizados para que sejam de fácil acesso para melhor experiência do usuário desde o aprendizado até o uso diário do sistema.

Sua arquitetura será baseada na arquitetura de microserviços onde será desenvolvida com o uso dos frameworks React e Django das linguagens JavaScript e Python, respectivamente.

Além dos frameworks e linguagens citados anteriormente, serão utilizados algumas ferramentas como forma de melhorar e organizar o processo de desenvolvimento do software, que são elas: Travis, Docker, GitHub e ZenHub.

## 10. Interfaces de Usuário
As seguintes telas serão disponibilizadas no sistema:
* Tela inicial
* Login
* Cadastro de empresas
* Lista de empresas
* Perfil da empresa
* Cadastro de funcionario
* Lista de funcionarios
* Perfil de funcionario
* Cadastro de nota fiscal
* Lista de notas fiscais
* Informações da nota fiscal
