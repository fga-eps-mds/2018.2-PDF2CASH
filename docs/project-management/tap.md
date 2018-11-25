# Termo de Abertura do Projeto (TAP)

## Histórico de Revisão

| Data | Versão | Descrição | Autor |
|:----:|:------:|:---------:|:-----:|
| 25/08/18 | 1.0 | Criação da TAP | Daniel Marques |
| 25/09/18 | 1.1 | Correção do resumo de custos | Daniel Marques |
| 25/11/18 | 2.0 | Revisão final | Carlos Aragon |

## 1. Introdução
Este documento tem como objetivo declarar o início do projeto e descrever a base do projeto PDF2CASH. Sendo assim, esse artefato disponibilizará informações como: visão de alto nível dos requisitos e riscos, limites e recursos, como também apresentam estudo sobre a viabilidade do produto, além dos dados sobre a equipe de desenvolvedores e engenheiros de produto.

## 2. Descrição do Projeto
O projeto PDF2CASH é um software desktop que automatiza o processo, especificamente, do setor financeiro de micro empresas. O processo na qual será automatizado é o gerenciamento de gastos da empresa por meio da gerência de notas fiscais.

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

![processo](/docs/assets/processo.jpg)

Para visualizar a imagem de forma ampliada [clique aqui](/docs/assets/processo.jpg)

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

## 7. Resumo do Orçamento (valor planejado)

O calculo do salário por hora foi calculado através da média de salário mensal no Brasil de cada profissão. Sendo que o profissional trabalharia 40 horas por semana e 1 mês há 5 semanas. Para visualizar as referências dos salários clique em um dos links abaixo:

[Programador de Software](https://www.catho.com.br/profissoes/programador-de-software):

    R$ 3.033,04 mensal
    R$ 15,16 por hora

[Engenheiro de Software](https://www.catho.com.br/profissoes/engenheiro-de-software):

    R$ 4.688,06 mensal
    R$ 23,34 por hora

* Programadores de Software:

      15 horas por semana * 5 semanas = 75
      R$ 15,16 por hora * 75 = R$ 1.137,00 por mês
      R$ 1.137,00 por mês * 4 meses = R$ 4.548,00 por integrante
      R$ 4.548,00 por integrante * 6 integrantes = R$ 27.288,00
 
* Engenheiros de Software:

      15 horas por semana * 5 semanas = 75
      R$ 23,34 por hora * 75 = R$ 1.758,00 por mês
      R$ 1.758,00 por mês * 4 meses = R$ 7.032,00 por integrante
      R$ 7.032,00 por integrante * 4 integrantes = R$ 28.128,00
 
* [Notebook](https://www.magazineluiza.com.br/notebook-asus-vivobook-15-x510ua-br540t-intel-core-i5-8gb-1tb-led-156-windows-10/p/220286100/in/note/?partner_id=4651&utm_source=google&utm_medium=pla&seller_id=magazineluiza&product_group_id=320285090761&ad_group_id=12602793504&aw_viq=pla&gclid=EAIaIQobChMIrPK0hJLh3QIVDBCRCh3z_gi2EAQYASABEgKCd_D_BwE): Asus Vivobook 15 X510UA-BR540T

      R$ 2.231,07 * 10 membros = R$ 22.310,70

* [Escritório](https://www.wimoveis.com.br/propriedades/comercial-asa-sul-2937221139.html?labs=I-spark-fav-filter-&labs_source=Recomendados_ficha_propiedad_desktop&itemid=2937183576&userid=0): 33 M² - Asa Sul

      aluguel = R$ 500,00
      condomínio = R$ 507,00
      R$ 500,00 + R$ 507,00 = R$ 1.007,00
      R$ 1.007,00 * 4 meses = R$ 4028,00

* [Internet corporativa](https://www.net.com.br/produtosnet/ofertanegocio_se3/?gclid=Cj0KCQjwxbzdBRCoARIsACzIK2nA0HYqxLZf2_J8sX014f135dqybDZ_2TRrF0sCT5ymyziKVLYSIccaAg2hEALw_wcB): NET - 140 mega

      R$ 155,00 * 4 meses = R$ 620,00
 
* Total:

      R$ 82.374,70

## 8. Partes Interessadas

### 8.1 Investidores

Micro empresas que querem automatizar seu setor financeiro para desenvolver a companhia frente aos concorrentes no mercado.

### 8.2 Equipe de Engenheiros de Software

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
