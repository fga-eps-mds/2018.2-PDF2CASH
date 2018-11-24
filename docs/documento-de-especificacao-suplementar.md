# PDF2Cash
***
# Especificação Suplementar
***
# Histórico da Revisão
| Data | Versão | Descrição | Autor |
|:----:|:------:|:---------:|:-----:|
| 09/09/18 | 0.1 | Abertura do documento de Especificação Suplementar | Lucas Gomes |
| 10/08/18 | 0.2 | Confiabilidade |  Brian Lui |
| 10/08/18 | 0.3 | Portabilidade |  Brian Lui |
| 11/08/18 | 0.4 | Desempenho | Lucas Gomes |
| 13/09/18 | 0.5 | Interoperabilidade | Julio Litwin |
| 13/09/18 | 0.6 | Segurança | Julio Litwin |
| 13/09/18 | 0.7 | Restrições de Design | Lucas Gomes |
| 13/09/18 | 0.8 | Introdução | Rafael Teodosio |
| 14/09/18 | 0.9 | Interface de usuário | Luís Cláudio T. Lima |
| 16/09/18 | 1.0 | Funcionalidades | Wictor Girardi|
| 20/09/18 | 1.1 | Revisão | Carlos Aragon|
| 23/11/18 | 1.2 | Revisão | Luís Cláudio T. Lima|

## 1.                  Introdução

### 1.1               Finalidade

Este documento tem como objetivo abordar aspectos técnicos, legais e demais requisitos sobre a aplicação PDF2CA$H, que não foram abordados nos demais documentos: Documento de Visão e Documento de Arquitetura.

### 1.2               Escopo

Os requisitos aqui explicados fazem parte do processo de desenvolvimento da aplicação web PDF2CA$H, que auxiliará diretores e funcionários de empresas de pequeno porte à controlar os gastos gerados por seus funcionários por meio de notas fiscais eletrônicas geradas em PDF.

### 1.3               Definições, Acrônimos e Abreviações

<table>
<th>Abreviação</td>
<th>Definição</td>
<tr><td>PDF</th>
<td>Portable Document Format</td>
</table>

### 1.4               Referências

## 2.                  Funcionalidade

Um ponto essencial para a usabilidade do sistema é que o mesmo ofereça um design e uma interação acessível para diretores e funcionários de empresas. Considerando o mais leigo dos usuários, o sistema deverá prezar pela simplicidade e acesso intuitivo, tendo em vista sua importância para o controle de gastos e uma utilização adequada pelos usuários da aplicação. Para alcançar tal meta, a aplicação deve conter um design limpo, de fácil visualização e entendimento, com acesso rápido e intuitivo a informações e funcionalidades importantes, sempre utilizando-se uma linguagem de fácil entendimento e compreensão.

### 2.1               Geração de gráficos

O sistema deve, de maneira automática, gerar gráficos baseados nos gastos condizente nas notas fiscais.

### 2.2               Arquivação de notas fiscais

O sistema deve arquivar, de maneira automática ou não, as notas fiscais que forem inseridas no programa.

### 2.3               Cadastro de funcionários

O sistema deve possuir uma maneira de cadastrar funcionários de empresas da qual a nota fiscal está sendo trabalhada.

### 2.4               Consulta no histórico de gastos

O sistema deve possuir uma maneira de gerar informações cronológicas de gastos com as notas fiscais.

### 3. Usabilidade

Um ponto essencial para a usabilidade do sistema proposto é que o mesmo ofereça um design e uma interação intuitiva e fácil para a parte financeira de uma empresa, para isso usaremos um design simples e objetivo, com acessos rápidos e diretos para todas as funcionalidades da aplicação. Nosso objetivo é que o programa seja facilmente usado por pessoas que não  necessitem de um treinamento específico para o uso, conseguindo operar o software sem maiores problemas com todas as suas funcionalidades. 	

### 3.1 Metas de usabilidade

#### Eficaz:
 O sistema deve fazer o que eu espero que faça, alcançar meu objetivo.
#### Eficiente:
 Velocidade de uso.
#### Segurança:
 Proteção ao usuário contra condições perigosas (monetárias e pessoais).
#### Utilidade:
Oferece o tipo certo de funcionalidade.
#### Aprendizado:
Fácil de aprender.
#### Memorização:
 Fácil de lembrar como se usa.
#### Prevenção de erros:
Evitar inserção de dados errôneos ou inadequados.
#### Diagnóstico de erro fácil para o usuário:
 Mensagens de erro claras e de fácil entendimento para o usuário.
#### Visibilidade de estado do sistema:
 Deixar claro ao usuário o que está acontecendo em tempo real.



## 4. Confiabilidade
Um dos requisitos para o bom funcionamento do sistema, será um alto nível de confiabilidade. De tal modo que a probabilidade da ocorrência de erros, falhas e bugs no sistema operacional seja mínima e que sejam sanadas o mais rápido possível.
O PDF2CASH poderá ser operado 24H por dia para que a manutenção seja contínua, e assim os erros serem corrigidos rapidamente para que não gere transtornos a empresa.

## 5. Desempenho
Deverá ser uma aplicação leve para que seja possível o uso do mesmo nas mais diferentes configurações de computadores e, também, terá que possuir um tempo de resposta rápido e preciso tanto com a elaboração de gráficos com os dados já adquiridos quanto com os dados presentes na nota fiscal.

## 6. Portabilidade
Para o uso do sistema será necessário que os dispositivos tenham o Sistem Operacional Linux. Poderá ser realizado o Download do programa em um dos seguintes navegadores com acesso a internet : Google Chrome, Mozilla Firefox.

## 7. Interoperabilidade
O PDF2CASH haverá conexão com banco de dados, utilizando-se o Sqlite3, onde serão armazenados dados de contas (administradores e usuários) e as notas fiscais processadas pelo PDF2CASH, com as informações exigidas. Sendo assim, tendo o banco de dados como um centro de informações e podendo chamar/atualizar/processar dados remotamente.

## 8. Segurança
Os dados no PDF2CASH apenas serão processados a partir de um controle de usuário, sendo assim, será necessário logar-se e ter os devidos privilégios na conta de usuário (sendo distinguindo em administrador e funcionário).

**Administrador** terá o seu papel em adicionar, excluir, editar e acessar funcionários, além de remover notas fiscais. Já o **Funcionário** será o responsável por gerenciar as notas fiscais.

Para mais informações, confira o **Documento de Arquitetura** - *Tópico: 4, Visão Geral*.

Nosso sistema busca incluir boas práticas de segurança de informações como: segurança de operações e comunicações, controle de acesso, autentição, dentre outros.

## 9. Restrições de Design
O PDF2CASH será uma aplicação minimalista e com cores que não tragam cansaço para a vista do usuário. As informações, links e botões serão organizados para que sejam de fácil acesso para melhor experiência do usuário desde o aprendizado até o uso diário do sistema.

Sua arquitetura será baseada em microserviços e será desenvolvida com o uso dos frameworks React e Django das linguagens JavaScript e Python, respectivamente.

Além dos frameworks e linguagens citados anteriormente, serão utilizados algumas ferramentas como forma de melhorar e organizar o processo de desenvolvimento do software, que são elas: Travis, Docker, GitHub e ZenHub.

## 10. Interfaces de Usuário
As seguintes telas serão disponibilizadas no sistema:
* Tela inicial
* Login
* Cadastrar funcionário
* Listar funcionarios
* Visualizar funcionário
* Cadastrar nota fiscal
* Listar notas fiscais
* Visualizar nota fiscal
