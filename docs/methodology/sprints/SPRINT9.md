# Sprint 09

## Histórico da Revisão
| Data | Versão | Descrição | Autor |
|:----:|:------:|:---------:|:-----:|
| 15/10/2018 | 0.1 | Planejamento da sprint | Daniel Marques |
| 22/10/2018 | 1.0 | Resultado da sprint | Daniel Marques |

## 1. Introdução

**Número da Sprint**: 9

**Data de Início**: 13/10/2018

**Data de Término**: 20/10/2018

**Duração**: 7 dias

**Pontos Planejados**: 22

**Pontos Adicionados (Dívida)**: 8

## 2. Papéis

**Scrum Master:**
* Daniel Marques

**Product Owner:**
* Carlos Aragon

**Arquiteto:**
* Bruno Matias

**DevOps:**
* Francisco Wallacy

**Desenvolvedores:**
* Brian Lui
* Julio Litwin
* Lucas Gomes
* Luís Cláudio
* Rafael Teodósio
* Wictor Girardi

## 3. Histórias Planejadas

As histórias podem ser vistas no [backlog do produto](https://github.com/fga-eps-mds/2018.2-PDF2CASH/blob/master/docs/methodology/backlog.md).


### 3.1. [EP03FE07TS06 - Refatorar Menu Lateral](https://github.com/fga-eps-mds/2018.2-PDF2CASH/issues/120) (3 pontos)

#### 3.1.1. Descrição

**Eu, como** desenvolvedor **desejo** refatorar o menu lateral **para** proporcionar uma interface mais acessível;

#### 3.1.2. Critério de Aceitação

* Deve permitir o acesso as funções principais do sistema a partir do menu lateral

#### 3.1.3. Responsáveis

* Brian Lui
* Wictor Girardi

### 3.2. [EP03FE07TS04 - Refatorar tabelas](https://github.com/fga-eps-mds/2018.2-PDF2CASH/issues/121) (3 pontos)

#### 3.2.1. Descrição

**Eu, como** desenvolvedor **desejo** refatorar formulários **para** proporcionar uma interface mais acessível e padronizada.

#### 3.2.2. Critério de Aceitação

* Formularios devem ser apresentados de forma simples e intuitiva

#### 3.2.3. Responsáveis

* Brian Lui
* Wictor Girardi

### 3.3. [EP02FE06TS07 - Refatorar parser (valor de imposto)](https://github.com/fga-eps-mds/2018.2-PDF2CASH/issues/110) (13 pontos)

#### 3.3.1. Descrição

**Eu, como** desenvolvedor **desejo** refatorar a parte de imposto do parser da nota fiscal **para** o sistema conseguir interpretar os dados de impostos adequadamente.

#### 3.3.2. Critério de Aceitação

* Informações definidas nas regras de negocio devem ser extraidas

#### 3.3.3. Responsáveis

* Lucas Gomes
* Julio Litwin

### 3.4. [EP01FE01US02 - Editar Funcionário](https://github.com/fga-eps-mds/2018.2-PDF2CASH/issues/109) (1 ponto)

#### 3.4.1. Descrição

**Eu, como** administrador ou funcionário **desejo** editar os dados da minha conta **para** manter os meus dados atualizados.

#### 3.4.2. Critério de Aceitação

* Deve ter o mesmo layout do formulário de cadastrar funcionário.

#### 3.4.3. Responsáveis

* Luis Claudio
* Rafael Teodósio

### 3.5. [EP01FE01US08 - Deletar nota fiscal](https://github.com/fga-eps-mds/2018.2-PDF2CASH/issues/) (2 pontos)

#### 3.5.1. Descrição

**Eu, como** administrador **desejo** deletar uma nota fiscal já registrada **para** apagar o registro de algum nota fiscal do sistema.

#### 3.5.2. Critério de Aceitação

* Quando deletar uma nota fiscal deve atualizar automaticamente a lista de notas fiscais.

#### 3.5.3. Responsáveis

* Luis Claudio
* Rafael Teodósio

## 4. Histórias Adicionadas (Dívida)

### 4.1. EP01FE08US15 - [Instalar o software](https://github.com/fga-eps-mds/2018.2-PDF2CASH/issues/102)	(8 pontos)

#### 4.1.1. Descrição

**Eu, como** administrador	**desejo** instalar o sistema em uma maquina	**para** ter acesso ao sistema.

#### 4.1.2. Critério de Aceitação

* Deve permitir o acesso ao sistema no fim da instalação.

#### 4.1.3. Responsáveis

* Bruno Matias
* Julio Litwin

## 5. Presença no Sprint Planning

| Presente | Membro |
|:--------:|:------:|
| S | Brian Lui |
| N | Bruno Matias |
| S | Carlos Aragon |
| S | Daniel Marques |
| N | Francisco Wallacy |
| S | Julio Litwin |
| N | Lucas Gomes |
| S | Luís Cláudio |
| S | Rafael Teodósio |
| S | Wictor Girardi |

## 6. Resultado

| ID | História | Status | Pontos |
|:--:|:--------:|:------:|:------:|
| EP03FE07TS06 | Refatorar Menu Lateral | Não Concluído | 3 |
| EP03FE07TS05 | Refatorar tabelas | Não Concluído | 3 |
| EP02FE06TS07 | Refatorar parser (valor de imposto) | Concluído | 13 |
| EP01FE01US02 | Editar Funcionário | Concluído | 1 |
| EP01FE01US08 | Deletar nota fiscal | Concluído | 2 |
| EP01FE08US15 | Instalar o software | Concluído | 8 |

**Pontos concluídos:** 24

**Pontos de dívidas:** 6

## 6.1. Burndown da Sprint

![Burndown Sprint 09](../../assets/burndown/burndown-sprint-09.png)

## 6.2. Velocity

![Velocity Sprint 09](../../assets/velocity/velocity09.png)

Para visualizar a imagem ampliada, [clique aqui](../../assets/velocity/velocity09.png).

## 6.3. Quadro de Conhecimentos

![Quadro de Conhecimento 09](../../assets/quadro-de-conhecimento/quadro09.png)

Para visualizar a imagem ampliada, [clique aqui](../../assets/quadro-de-conhecimento/quadro09.png).

### 6.4. Retrospectiva:

| Negativo | Positivo | Melhoria |
|:--------:|:--------:|:--------:|
| Alguma integrantes do time deixaram para implementar no último instante da sprint as respectivas histórias | Duas histórias foram concluídas no ínicio da sprint | Começar a implementar as histórias no ínicio da sprint, após essa época de provas |
| Foi concluída a maioria das histórias | O layout está muito mais chamativa para o usuário após a refatoração | Realizar teste de aceitação no front |
| A grande maioria dos integrantes da equipe estava com provas na semana |  |  |
| Duas histórias estavam implementadas mas os responsáveis não mandaram pull request |  |  |
| O front ainda está sem uma ferramenta para teste |  |  |

### 6.5. Retrospectiva do Scrum Master:

Como uma das dificuldades que ocorreu foi as várias provas que aconteceram durante a semana para alguns integrantes, acabou aumentando a dificuldade de implementar as histórias dessa sprint, sendo isso visto nas duas histórias não concluídas ("[EP03FE07TS06 - Refatorar Menu Lateral](https://github.com/fga-eps-mds/2018.2-PDF2CASH/issues/120)" e "[EP03FE07TS04 - Refatorar tabelas](https://github.com/fga-eps-mds/2018.2-PDF2CASH/issues/121)"). Mas em contra partida a história mais difícil e importante da sprint foi concluída com sucesso que é a "[EP02FE06TS07 - Refatorar parser (valor de imposto)](https://github.com/fga-eps-mds/2018.2-PDF2CASH/issues/110)", na qual o parser teria que ser refatorado para resgatar a parte de frete/impostos do pdf da nota fiscal, que anteriormente não estava pegando tais informações. 

O parser está pegando a grande parte das informações do pdf, mas pode-se notar a demora ao requisitar a funcionalidade de "Criar fota fiscal", causado exatamente pelo conversor em python usado. A equipe está estudando um outro conversor que possa ser utilizado no lugar, que provavelmente será em C++ utilizando Qt.

### 6.6. Presença no Sprint Review

| Presente | Membro |
|:--------:|:------:|
| S | Brian Lui |
| N | Bruno Matias |
| N | Carlos Aragon |
| S | Daniel Marques |
| S | Francisco Wallacy |
| S | Julio Litwin |
| S | Lucas Gomes |
| S | Luís Cláudio |
| S | Rafael Teodósio |
| S | Wictor Girardi |
