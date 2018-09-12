# Documento de visão
***
## Histórico de Revisão
***

| Data | Versão | Descrição | Autor |
|:----:|:------:|:---------:|:-----:|
| 25/08/18 | 0.1 | Abertura do Documento de Visão | Brian Lui |
| 26/08/18 | 0.2 | Introdução | Brian Lui |
| 28/08/18 | 0.3 | Posicionamento | Wictor Girardi |
| 29/08/18 | 0.4 | Visão Geral Do Produto | Rafael Teodosio |
| 31/08/18 | 0.5 | Descrição dos Envolvidos e dos Usuários | Lucas Gomes |
| 03/09/18 | 0.5.1 | Mudança dentro do posicionamento | Wictor Girardi |
| 03/09/18 | 0.6 | Adição de Descrição dos Envolvidos e dos Usuários | Lucas Gomes |
| 05/09/18 | 0.7 | Adição de recursos do produto | Wictor Girardi |
| 05/09/18 | 0.8 | Restrições | Julio Litwin |
| 05/09/18 | 0.9 | Intervalos de Qualidade | Luis Claudio T. Lima |

***
## 1. Introdução
***

Esta documentação tem como propósito coletar, analisar e definir os insumos necessários para a realização do PDF2K, que é uma ferramenta para gerar dados a partir de notas fiscais eletrônicas(NFe). Sendo possível o armazenamento, organização e geração de NFe. 
Nesta introdução será apresentada uma visão geral para o total entendimento do projeto, de tal modo que fique claro para todos os recursos necessários e as razões que levam a essas necessidades.

### 1.1 Finalidade

Este documento tem como objetivo definir todos os requisitos, necessidades e os recursos necessários, especificamente as de alto nível,  para que o cliente possa compreender e tenha o completo entendimento do projeto PDF2K.

### 1.2 Escopo

Neste documento serão abordados os pontos necessários para o desenvolvimento do PDF2K, na qual será utilizado na parte financeira gerando dados a partir de notas fiscais eletrônicas e assim controlar o fluxo de caixa de determinada empresa, de tal modo que pessoas que não possuam o conhecimento técnico da tecnologia utilizada possam entender sem problemas. 

### 1.3 Definições, Acrônimos e Abreviações

Alguns termos e conceitos serão necessários saber para o total entendimento deste documento e que estarão listadas logo abaixo :

PDF(Portable Document Format): É um formato de arquivo usado para exibir e compartilhar documentos de maneira compatível.
NFe: Nota Fiscal Eletrônica
HD(Hard Disk): Sistema de armazenamento de alta capacidade destinado ao armazenamento de arquivos e programas.
PO: Product Owner
IA: inteligência artificial 
CTe: Conhecimento de Transporte Eletrônico
CNPJ: Cadastro Nacional da Pessoa Jurídica
Backup: Cópia de segurança

### 1.4 Referências

WARNOCK, John. Adobe. Disponível em: <https://acrobat.adobe.com/br/pt/acrobat/about-adobe-pdf.html>. Acesso em: 29 ago. 2018.

### 1.5 Visão Geral

Neste documento é definido o problema a ser resolvido de acordo com os requisitos do software previamente elaborados, o entendimento sobre os usuários e envolvidos, uma visão geral do produto a ser desenvolvido e dos recursos necessários.

***
## 2. Posicionamento
***

### 2.1 Oportunidade de Negócios

Atualmente diversas empresas enfrentam problemas relacionados ao seus controles de gastos e com consequência disso ocorre a dificuldade de maximização de lucros, levando em consideração o grande volume de vendas e compras realizados, e algumas vezes por falta de experiência na coordenação econômica da empresa. Com base nesses problemas o PDF2K busca realizar de maneira rápida e prática a organização, armazenamento e geração de gráficos de dados baseados nas notas fiscais recebidas por essas empresas, gerando assim um maior controle de onde está sendo gasto o dinheiro e se está ocorrendo aumentos ou quedas no histórico monetário dessa empresa além da prevenção de possíveis multas causadas pela falta de armazenamento das notas fiscais.

### 2.2 Descrição do Problema

<table>
  <tr><th>O problema de</th><td>Falta de praticidade no trabalho relacionado às notas fiscais que abrange a falta de organização e a falta de controle de gastos </td></tr>
  <tr><th>Afeta</th><td>
A empresa de modo geral e principalmente seu setor financeiro
</td></tr>
  <tr><th>Cujo impacto é</th><td>O setor financeiro da empresa já que não consegue de maneira prática manter a organização e controle de seus gastos e o armazenamento de suas notas fiscais, causando dano ao lucro geral da empresa</td></tr>
  <tr><th>Uma boa solução seria</th><td>Uma aplicação prática e inteligente que por meio de artifícios de IA e aprendizado de máquina reconhece notas fiscais emitidas e trabalha em cima delas, gerando de maneira automatizada gráficos de  gastos recentes ou mesmo dentro de um histórico, gerando um melhor entendimento de onde e porque está sendo gasto o dinheiro da empresa, juntamente com o armazenamento automático dessas notas, evitando assim burocracia e trabalho desnecessário realizando uma maximização de lucros da empresa</td></tr>
</table>


### 2.3 Sentença de Posição do Produto

<table>
  <tr><th>Para</th><td>Empresas e negócios, com ênfase no setor financeiro </td></tr>
  <tr><th>Que</th><td>
Possuem a necessidade de um software que realize de maneira automatizada, prática e organizada o controle de gastos por meio de gráficos, organização de notas fiscais sem a necessidade de interação humana durante o processo
</td></tr>
  <tr><th>O (nome do produto)</th><td>PDF2CASH</td></tr>
  <tr><th>Diferente de</th><td>Noov e Arquivei</td></tr>
  <tr><th>Nosso produto</th><td>Gera dados úteis baseando-se na leitura nativa de arquivos PDF’s de notas fiscais de maneira automática e rápida, agrupando os gastos relacionados, gerando gráficos de história e realizando um armazenando seguro das notas fiscais </td></tr>
</table>

***
## 3. Descrições dos Envolvidos e dos Usuários
***

### 3.1 Resumo dos Envolvidos
| Nome | Descrição | Responsabilidades |
|:----:|:---------:|:-----------------:|
| Investidores | Micro empresas com interesse em automatizar o controle de notas fiscais | Avaliar a qualidade do produto no intuito de comprar o mesmo. |
| Equipe de desenvolvimento do projeto | Equipe de alunos de Métodos de Desenvolvimento de Software da UnB | Planejar, desenvolver, testar, documentar e implementar o sistema. |
| Equipe de engenharia de produto | Equipe de alunos de Engenharia de Produto de Software da UnB | Planejar, projetar e gerir o projeto. Onde a equipe é composta pelo PO, Scrum Master, DevOps e Arquiteto que desempenham os papéis de, respectivamente, compreender, guiar a equipe, estudar a implementação e, configurar o ambiente de desenvolvimento do projeto. |

### 3.2 Resumo dos Usuários
| Nome | Descrição | Responsabilidades | Envolvido |
|:----:|:---------:|:-----------------:|:---------:|
| Administrador | Operador do sistema com mais recurso para uso | Responsável por realizar cadastro de novos usuários e empresas | Usuário |
| Usuário Comum | Operador do sistema | Responsável pelo “upload” das notas fiscais e fará uso da aplicação | Usuário |

### 3.3 Perfis dos Envolvidos

#### 3.3.1	Investidores
<table>
  <tr><th>Representante</th><td>Investidor</td></tr>
  <tr><th>Descrição</th><td>Investidor com o interesse em automatizar o gerenciamento de notas fiscais da empresa.</td></tr>
  <tr><th>Tipo</th><td>Conhecimento na área administrativa e financeira</td></tr>
  <tr><th>Responsabilidades</th><td>Observar e dar sua opinião sobre a aplicação</td></tr>
  <tr><th>Critérios de Sucesso</th><td>Receber uma aplicação que possa suprir suas necessidades diante as notas fiscais de forma automatizada.</td></tr>
  <tr><th>Envolvimento</th><td>Alto</td></tr>
  <tr><th>Comentários / Problemas</th><td>-</td></tr>
</table>

#### 3.3.2	Equipe de Desenvolvedores
<table>
  <tr><th>Representante</th><td>Brian Lui<br>
  Julio Cesar Litwin<br>
  Lucas Gomes Silva<br>
  Luis Claudio Telles Lima<br>
  Rafael Santos Teodosio<br>
  Wictor Bastos Girardi<br></td></tr>
  <tr><th>Descrição</th><td>Desenvolvedores do projeto</td></tr>
  <tr><th>Tipo</th><td>Graduandos de Engenharia de Software na Universidade de Brasília, matriculados na disciplina de Métodos de Desenvolvimento de Software</td></tr>
  <tr><th>Responsabilidades</th><td>Planejar o sistema, realizar testes de implementação, documentar a estrutura do software e implementar o sistema de acordo com a documentação.</td></tr>
  <tr><th>Critérios de Sucesso</th><td>Desenvolver o sistema dentro do prazo estimado e adquirir novos conhecimentos sobre desenvolvimento de software.</td></tr>
  <tr><th>Envolvimento</th><td>Alto</td></tr>
  <tr><th>Comentários / Problemas</th><td>-</td></tr>
</table>

#### 3.3.3	Equipe de Desenvolvedores
<table>
  <tr><th>Representante</th><td>Bruno Matias Casas<br>
  Carlos Enrique Rodrigues Aragon<br>
  Daniel Marques Rangel<br>
  Francisco Wallacy Coutinho Braz<br></td></tr>
  <tr><th>Descrição</th><td>Engenheiros de Produto de Software</td></tr>
  <tr><th>Tipo</th><td>Graduandos de Engenharia de Software na Universidade de Brasília, matriculados na disciplina de Engenharia de Produto de Software</td></tr>
  <tr><th>Responsabilidades</th><td>Planejar o projeto, programar os recursos definidos do projeto e gerir a equipe de desenvolvedores. A equipe é composta pelo Product Owner, Scrum Master, DevOps e Arquiteto que desempenham os papéis de, respectivamente, compreender o mercado e vender a idéia ao investidor, guiar e facilitar as tarefas realizadas pela equipe, configurar o ambiente de desenvolvimento do projeto e estudar formas de implementação do sistema por completo.</td></tr>
  <tr><th>Critérios de Sucesso</th><td>Entregar a aplicação no tempo estimado, vender a idéia da aplicação aos investidores e aumentar a experiência na área de desenvolvimento de software e gestão de projeto.</td></tr>
  <tr><th>Envolvimento</th><td>Alto</td></tr>
  <tr><th>Comentários / Problemas</th><td>-</td></tr>
</table>

### 3.4 Perfis dos Usuários

#### 3.4.1 Administrador

<table>
  <tr><th>Representante</th><td>Usuários</td></tr>
  <tr><th>Descrição</th><td>Funcionários que fazem parte da administração da área financeira ou de confiança  da empresa</td></tr>
  <tr><th>Tipo</th><td>Usuário avançado</td></tr>
  <tr><th>Responsabilidades</th><td>Conhecer a aplicação de modo que possa organizar os PDFs presentes na aplicação, gerar relatórios, adicionar novas empresas ao sistema e realizar o cadastro de novos usuários.</td></tr>
  <tr><th>Critérios de Sucesso</th><td>Receber um sistema capaz de automatizar tarefas repetitivas que envolvem notas fiscais</td></tr>
  <tr><th>Envolvimento</th><td>Usuário final do sistema</td></tr>
  <tr><th>Comentários / Problemas</th><td>-</td></tr>
</table>

#### 3.4.2 Administrador

<table>
  <tr><th>Representante</th><td>Usuários</td></tr>
  <tr><th>Descrição</th><td>Funcionários que fazem parte do setor financeiro ou de confiança da empresa</td></tr>
  <tr><th>Tipo</th><td>Usuário comum</td></tr>
  <tr><th>Responsabilidades</th><td>Conhecer a aplicação de modo que possa organizar os PDFs presentes na aplicação e gerar relatórios</td></tr>
  <tr><th>Critérios de Sucesso</th><td>Receber um sistema capaz de automatizar tarefas repetitivas que envolvem notas fiscais</td></tr>
  <tr><th>Envolvimento</th><td>Usuário final do sistema</td></tr>
  <tr><th>Comentários / Problemas</th><td>-</td></tr>
</table>

### 3.5 Principais Necessidades dos Usuários ou dos Envolvidos

| Necessidade | Prioridade | Preocupações | Solução Atual | Soluções Propostas |
|:---:|:---:|:---:|:---:|:---:|
| Agilidade e automatização na análise e organização de notas fiscais | Alta | Falta de agilidade na análise das notas fiscais e possíveis erros humanos | Verificação manual das notas fiscais | Realizar a leitura da nota fiscal com o auxílio de aprendizagem de máquina ou divisão da nota fiscal por blocos onde as notas são adicionadas para serem lidas de forma automática |
| Gerar relatórios com base nas notas fiscais recebidas | Alta | Possíveis erros humanos na hora da elaboração do relatório | Feito de forma manual | De acordo com a leitura feita nas notas fiscais, a aplicação gerará relatórios conforme a necessidade do usuário |

### 3.6 Alternativas e Concorrência

#### 3.6.1 Noov
É uma plataforma web gratuito onde é possível realizar o armazenamento de NFes que garante o backup seguro de suas notas na nuvem tendo também a opção de envio ou recebimento de notas fiscais de forma automática. O Noov permite também compartilhar as notas fiscais da empresa com seus clientes, parceiros e contadores. Esse portal possui uma API voltada a desenvolvedores com o intuito de desenvolverem novos aplicativos e colaborarem com a plataforma Noov.

![Noov](https://uploaddeimagens.com.br/images/001/604/543/original/Noov.png?1536550429)


#### 3.6.2 Arquivei
Desenvolvido e mantido por uma startup constituída por alunos e ex-alunos da Universidade de São Paulo, o Arquivei é uma plataforma web paga que tem como objetivo o acesso fácil aos documentos fiscais da empresa. A plataforma é conectado à Secretaria da Fazenda e baixa automaticamente todas as NFes e CTes emitidas para o CNPJ da empresa, armazenando-as no painel de gestão de notas da plataforma. Todas informações presentes na plataforma se tornam gráficos para melhor visualização do usuário. O Arquivei possui três planos de contratação com taxas mensais: o primeiro, Plano Starter, no valor de R$ 29,90; o segundo com o nome de Plano Controle no valor de R$ 49,90 e; o terceiro plano, intitulado Plano Business, possuindo o valor de R$ 89,90.

![Arquivei](https://uploaddeimagens.com.br/images/001/604/545/original/Arquivei.png?1536550547)


***
## 4.                  Visão Geral do Produto
***

### 4.1               Perspectiva do Produto

O PDF2K irá sistematizar o processo de leitura e transformação de arquivos (PDF). De tal forma que, Diretores e funcionários da empresa tenham o controle sobre seus gastos. O produto fornecerá aos usuários as informações necessárias para melhor gerirem a parte financeira. Tais informações contemplam categoria de gastos, valores unitários, valores totais, análise de dados, margem de gastos, histórico de gastos . Assim, têm-se como expectativa facilitar, agilizar o processo de controle fiscal, além de ampliar os lucros pelo fato de ter-se um controle automatizado dos gastos.

### 4.2               Resumo dos Recursos

<table>

  <tr><th>Benefício para o Cliente</th><th>Recursos de Suporte</td></tr>
  <tr><td>Agilidade no processamento dos dados sem a necessidade da criação de planilhas.</th><td>Uma base de conhecimentos ajuda o pessoal de suporte a identificar rapidamente ações corretivas e soluções conhecidas.</td></tr>
  <tr><td>O usuário poderá descobrir em que ou onde é o seu maior gasto, podendo assim melhorar o seu planejamento financeiro.</th><td>Os problemas são relacionados como itens únicos, classificados e monitorados ao longo de todo o processo de resolução. São emitidas notificações automáticas para os problemas que têm seus prazos expirados.
  </td></tr>
  <tr><td>A margem de gastos calculada dará ao usuário uma noção do quanto será o gasto estimado do mês, semana ou ano.
  </th><td>Os relatórios de tendências e de distribuição permitem revisões de nível superior do status dos problemas.
  </td></tr>
  <tr><td>
  Os clientes têm autonomia para resolver seus problemas, o que reduz os custos de suporte e melhora o tempo de resposta.
  </td></th>
  </th><td>Um servidor de duplicação permite que as informações atuais do banco de dados sejam compartilhadas pela empresa.
  </td></tr>
</table>

### 4.3               Custos e Preços

### 4.4               Licenciamento e Instalação

A instalação será realizada de forma interativa e simples por meio de um instalador, que será disponibilizado no site oficial do produto, o mesmo será compatível com os sistemas Windows sendo necessário espaço no HD o suficiente para concluir a instalação.
O licenciamento do produto estará vinculado à sua conta associada ao produto sendo diferenciada através de funcionalidades, abrangendo assim uma gama de usuários maior atendendo suas necessidades.

***
## 5. Recursos do Produto
***

### Legenda de Prioridades dos Requisitos:

<table>
  <tr><th>Prioridade</th><th>Caracteristica</td></tr>
  <tr><td>Alta</th><td>Requisito fundamental para o sistema </td></tr>
  <tr><td>Intermediaria</th><td>Requisito importante, mas não é fundamental para o funcionamento do sistema</td></tr>
  <tr><td>Baixa</th><td>Requisito não fundamental e pouco usado no sistema</td></tr>

</table>


| Identificador| Nome | Descrição | Prioridade |
|:----:|:---------:|:-----------------:|:--------|
| RF1 | Geração de gráficos  |O sistema de maneira automática deve gerar gráficos baseados nos gastos condizente nas notas fiscais. | Alta |
| RF2 | Arquivação de notas fiscais | O sistema deve arquivar de maneira automática ou não as notas fiscais que forem inseridas no programa | Alta |
| RF3 | Cadastro da empresa | O sistema deve possuir uma maneira de cadastrar aa empresa da qual a nota fiscal está sendo trabalhada | Alta |
| RF4 | Consulta no histórico de gastos | O sistema deve possuir uma maneira de gerar informações cronológicas de gastos com as notas fiscais | Media

***
## 7. Intervalos de Qualidade
***

### 7.1   Requisitos de Sistema
* O sistema consiste em uma aplicação desktop na qual é necessário acesso a uma rede estável para a conexão com o servidor.
* Deve ser possível instalar a aplicação desktop nos seguintes sistemas operacionais: Windows, distribuições Linux e MacOS.

### 7.2   Requisitos de Desempenho
* O sistema deve ter o tempo de execução e resposta de acordo com a qualidade da conexão de internet, sendo assim, a velocidade de rede irá impactar diretamente o sistema em todas as suas funcionalidades.
* O sistema deve suportar no mínimo 100 usuários possíveis.

### 7.3   Requisitos de Design
* O sistema deve ter uma interface organizada e intuitiva suficiente para o uso adequado, tendo também cores indicadoras que possam diferenciar cada funcionalidade.

### 7.4   Requisitos de Confiabilidade      
* O sistema deve calcular com precisão o valores de cada item na nota fiscal.
* O sistema deve poder se recuperar de falhas que possam ocorrer durante a sua utilização.

### 7.5   Requisitos de Arquitetura
* O sistema deve possuir uma arquitetura orientada a micro serviços.
* O sistema deve seguir a modelagem definida pelo arquiteto da equipe.

### 7.6   Requisitos de Usabilidade
* A interface do sistema deve ser responsivo de acordo com o tamanho de tela do usuário.
* A interface do sistema deve instruir o usuário no preenchimento de campos de formulários.
* O sistema deve exibir notificações caso tenha erro ou sucesso no preenchimento do formulário.

### 7.7   Requisitos de Suportabilidade
* Nesse sistema deve ser possível fazer a instalação no sistema do usuário para a execução do mesmo.
* O sistema deve seguir o padrão de codificação criado pelo integrate devops da equipe.

### 7.8   Requisitos de Segurança
* O sistema deve armazenar e administrar os dados dos funcionários de forma a garantir a privacidade dos mesmos.
* O sistema deve impedir o acesso de pessoas não autorizadas.
* O sistema deve possuir validação para cada dado inserido no banco de dados.
