# Termo de Abertura do Projeto (TAP)

## Histórico de Revisão

| Data | Versão | Descrição | Autor |
|:----:|:------:|:---------:|:-----:|
| 25/08/18 | 0.1 | Criação da TAP | Daniel Marques |

## 1. Introdução
Este documento tem como objetivo declarar o início do projeto e descrever a base do projeto PDF2CASH. Sendo assim, neste artefato terá informações como: visão de alto nível dos requisitos e riscos, limites e recursos, como também apresentam estudo sobre a viabilidade do produto, além dos dados sobre a equipe de desenvolvedores e engenheiros de produto.

## 2. Descrição do Projeto
O projeto PDF2CASH é um software desktop que automatiza o processo, especificamente, do setor financeiro de micro empresas. O processo na qual será automatizado é o gerenciamento de gastos feitos pela empresa por meio da nota fiscal.

## 3. Problemas e Solução do Projeto
Como o setor financeiro é considerado o “coração” de uma empresa, é necessário sempre procurar melhorar os processos dessa parte, caso queira que a empresa cresça para competir no mercado com vários outros concorrentes. E um dos problemas encontrados é o gerenciamento de gastos, na qual é contabilizado as notas fiscais recebidas de forma manual, ocorrendo assim, erros humanos como por exemplo: valor total  lançado errado, itens da nota fiscal anotados de modo equívoco etc.
O software trará como solução: automatizar leitura de notas fiscais, armazenar os dados de cada nota fiscal e disponibilizar análises financeiras das notas fiscais lidas. Com isso, reduzindo significativamente a quantidade de trabalho manual e possíveis erros humanos se comparado ao processo manual.

## 4. Requisitos de Alto Nível
O produto PDF2CASH tem como objetivo principal automatizar o processo de gerenciamento e contabilidade de notas fiscais no setor financeiro de micro empresas. Esse software deverá prover:
* Sistema de sessão para cada usuário
* Manter contas de usuários por meio do administrador
* Adicionar, visualizar e excluir nota fiscal
* Manter análises financeiras
* Adicionar, visualizar e editar empresa

## 5. Riscos de Alto Nível
Dentre os riscos do projeto estão:
* Integrantes não cumprirem os deveres de seus devidos papéis na metodologia utilizada, seja por falta de conhecimento do papel realizado pelo integrante ou negligência do mesmo, resultando em atraso o término do sistema. Se ocorrer, será feita uma reunião comunicando o ocorrido, averiguando o motivo e corrigindo as atividades do integrante as atividades definidas anteriormente.
* Alta taxa de defeitos no ambiente de homologação, causado geralmente por implementações realizadas de forma rápida e descuidada. Para prevenir, as implementações deverão ser aceitas pelo Product Owner antes de serem aplicadas em ambiente de homologação. Se acontecer, será feito TS’s (technical storie’s) para fazer as devidas correções nos problemas encontrados.
* O plano de comunicação não ser efetivo, trazendo um fluxo de informações falho sobre os dados de implementação, aumentando erros humanos sobre o projeto. Na eventualidade de surgir, o plano de comunicação será reformulado.
* Membros não dominarem as tecnologias utilizadas no produto, desta forma, atrasaria a entrega do produto. Na hipótese de acontecer, será dado mais treinamentos sobre as tecnologias.
* Algum ou vários integrantes abandonarem o projeto, assim, prejudicando os outros membros da equipe. Caso isso aconteça, será feito mudanças no cronograma das atividades propostas, ou seja, redistribuir cada atividade pendente entre os membros restantes, para assim, chegar na conclusão do software.

## 6. Resumo do Cronograma
O prazo para construção do produto será de 16 semanas, totalizando 112 dias de trabalho. Sendo que será dividido em duas etapas: a primeira será entre a “Iniciação” e a primeira entrega, chamada de “Release 01”, a segunda será após a “Release 01” até a segunda entrega, chamada “Release 02”. As datas podem ser vistas na tabela abaixo:

| Marcos | Previsão |
|:------ |:--------:|
| Iniciação | 14/08/2018 |
| Release 01 | 02/09/2018 |
| Release 02 | 06/12/2018 |

![processo](assets/processo.jpg)

Para visualizar a imagem de forma ampliada [clique aqui](assets/processo.jpg)

O foco da primeira etapa estará nas seguintes atividades:
* Definição do escopo do projeto.
* Estudo das tecnologias a serem utilizadas.
* Definição da metodologia a ser usada.
* Configuração de ambiente, junto com integração contínua e deploy automático.
* Documentação do escopo, da implementação, da configuração e da metodologia.
* Protótipo.
* Implementação do gerenciamento de sessão e manter usuário pelo administrador para entregar na Release 01.
* Testar a implementação.

Já na segunda etapa será as seguintes atividades:
* Protótipo.
* Implementação das outras funcionalidades do software.
* Testar a implementação.

## 7. Resumo do Orçamento

O salário médio para Desenvolvedor de Software Full Stack é de **R$ 4.850**/mensal.

O salário médio para Engenheiro de Produto Júnior é de **R$ 7.691**/mensal.
 
* Desenvolvedores:
    R$ 4.850,00 * 6 desenvolvedores * 4 meses = **R$ 116.500,00**
 
* Devops:
      R$ 7.691,00 * 4 devops * 4 meses = **R$ 123.056,00**
 
* Notebooks:
      R$ 2.500,00 * 10 membros = **R$ 25.000,00**
 
* Moradia:
      R$ 500,00 * 4 meses = **R$ 2000,00**
 
* Internet:
      R$ 120,00 * 4 meses = **R$ 480,00**
 
* Energia:
      R$ 200,00 * 4 meses = **R$ 800,00**
 
* Total:
      **R$ 267.836,00**

## 8. Partes Interessadas

### 8.1 Investidores

Micro empresas que querem automatizar seu setor financeiro para desenvolver a companhia frente aos concorrentes no mercado.

### 8.2 Equipe de Engenheiros de Produção

A equipe é composta pelo Product Owner, Scrum Master, DevOps e Arquiteto que desempenham os papéis de, respectivamente, compreender o mercado e vender a idéia ao investidor, guiar e facilitar as tarefas realizadas pela equipe, configurar o ambiente de desenvolvimento do projeto e estudar formas de implementação do sistema por completo.

| Nome | E-mail | Github |
| ---- | ------ |:------:|
| Bruno Matias Casas | brunomatiascasas@hotmail.com | @Matias0422 |
| Carlos Enrique Rodrigues Aragon | carlosaragon3@hotmail.com | @carlosaragon |
| Daniel Marques Rangel | danielmarques7@hotmail.com | @danielmarques28 |
| Francisco Wallacy Coutinho Braz | wallacy.braz@live.com | @wallacybraz |

### 8.3 Equipe de Desenvolvimento

Membros da equipe que tem a responsabilidade de documentar parte do software, implementar e testá-lo e seguir a documentação relacionada às metodologias definidas.

| Nome | E-mail | Github |
| ---- | ------ |:------:|
| Brian Lui | brianlui2387@gmail.com | @Brian2397 |
| Julio Cesar Litwin | j.litwin@live.com | @jclitwin |
| Lucas Gomes Silva | lucas.gomesgs0@gmail.com | @lucasgomesgs0 |
| Luis Claudio Telles Lima | lclaudio.tl@gmail.com | @LuisCL94 |
| Rafael Santos Teodosio | rafael.s.t@hotmail.com | @rafaelteodosio |
| Wictor Bastos Girardi | wictor.girardi@gmail.com | @Wictorgirardi |
