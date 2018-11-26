# Backlog do Produto

## Histórico de Revisão

| Data | Versão | Descrição | Autor |
|:----:|:------:|:---------:|:-----:|
| 15/09/18 | 1.0 | Criação do backlog | Daniel Marques |
| 26/09/18 | 1.1 | Adicionado tabela de TS, correção dos pontos de complexidade, adicionado total de pontos e remoção da Feature "Manuntenção de Empresa" | Daniel Marques |
| 16/10/18 | 1.2 | Atualização das us e ts | Carlos Aragon |
 | 24/11/18 | 2.0 | Atualização das us e ts | Carlos Aragon |

## Total de Pontos

| Tipo | Pontos |
|:----:|:------:|
| US | 82 |
| TS | 135 |
| TOTAL | 217 |

## User Stories

Abaixo está descrito as histórias de usuário:

<table border="2">
  <tr>
    <th>ÉPICO</th>
    <th>FEATURE</th>
    <th>US</th>
    <th>FUNCIONALIDADE</th>
    <th>EU, COMO...</th>
    <th>DESEJO...</th>
    <th>PARA...</th>
    <th>PRIORIDADE</th>
    <th>PONTUAÇÃO</th>
    <th>STATUS</th>
  </tr>
  <tr style="color:green">
    <td rowspan="11">EP01 - Usuário</td>
    <td rowspan="5">FE01 - Manuntenção do Funcionário</td>
    <th>US01</th>
    <td>Criar funcionário</td>
    <td>administrador</td>
    <td>criar a conta de um funcionário</td>
    <td>o funcionário ter acesso aos dados financeiros da empresa dentro do sistema</td>
    <td>Should</td>
    <td >5</td>
    <td >Concluída</td>
  </tr>
  <tr style="color:green">
    <th >US02</th>
    <td >Editar funcionário</td>
    <td >administrador ou funcionário</td>
    <td >editar os dados da minha conta</td>
    <td >manter os meus dados atualizados</td>
    <td >Should</td>
    <td >1</td>
    <td >Concluída</td>
  </tr>
  <tr style="color:green">
    <th>US03</th>
    <td>Deletar funcionário</td>
    <td>administrador</td>
    <td>deletar a conta de um funcionário</td>
    <td>apagar conta não utilizada mais</td>
    <td>Should</td>
    <td >2</td>
    <td >Concluída</td>
  </tr>
  <tr style="color:green">
    <th >US04</th>
    <td >Visualizar funcionário</td>
    <td >administrador</td>
    <td >visualizar a conta de um funcionário</td>
    <td >ter conhecimento dos dados do funcionário e a empresa relacionada a ele</td>
    <td >Should</td>
    <td >5</td>
    <td >Concluída</td>
  </tr>
  <tr style="color:green">
    <th>US05</th>
    <td>Listar funcionários</td>
    <td>administrador</td>
    <td>visualizar a lista de contas de funcionários</td>
    <td>ter conhecimento dos funcionários registrados</td>
    <td>Should</td>
    <td>3</td>
    <td>Concluída</td>
  </tr>
  <tr style="color:green">
    <td rowspan="2">FE05 - Configuração da conta</td>
    <th span style="color:red"> US06</th>
    <td style="color:red">Editar Perfil</td>
    <td style="color:red">administrador ou funcionário</td>
    <td style="color:red">editar os dados do meu perfil</td>
    <td style="color:red">atualizar os dados como por exemplo nome e senha</td>
    <td style="color:red">Could</td>
    <td style="color:red">3</td>
    <td style="color:red">Removido</td>
  </tr>
  <tr style="color:green">
    <th>US16</th>
    <td>Cadastrar administrador</td>
    <td>administrador</td>
    <td>criar uma conta para mim</td>
    <td>ter acesso ao sistema como administrador</td>
    <td>Must</td>
    <td>13</td>
    <td>Concluída</td>
  </tr >
    <tr style="color:green">
    <td rowspan="2">FE04 - Sessão</td>
    <th>US13</th>
    <td>Fazer login</td>
    <td>administrador ou funcionário</td>
    <td>entrar na minha conta</td>
    <td>para ter acesso ao sistema</td>
    <td>Should</td>
    <td>8</td>
    <td >Concluída</td>
  </tr>
  <tr style="color:green">
    <th >US14</th>
    <td >Fazer logout</td>
    <td >administrador ou funcionário</td>
    <td >sair da minha conta</td>
    <td >poder encerrar a minha sessão</td>
    <td >Should</td>
    <td >2</td>
    <td >Pendente</td>
  </tr>
  <tr style="color:green">
    <td rowspan="2">FE08 - Instalação</td>
    <th >US15</th>
    <td >Instalar o software</td>
    <td >administrador</td>
    <td >instalar o sistema em uma maquina</td>
    <td >para ter acesso ao sistema</td>
    <td >Must</td>
    <td >2</td>
    <td >Concluída</td>
  </tr>
  <tr style="color:green">
    <th >US16</th>
    <td >Atualizar a aplicação</td>
    <td >administrador ou funcionário</td>
    <td >atualizar aversão do sistema</td>
    <td >utilizar a versão mais recente do software</td>
    <td >Should</td>
    <td >13</td>
    <td>Concluída</td>
  </tr>
  <tr style="color:green">
    <td rowspan="9">EP02 - Financeiro</td>
    <td rowspan="4">FE02 - Manuntenção da nota fiscal</td>
    <th>US07</th>
    <td>Criar nota fiscal</td>
    <td>administrador ou funcionário</td>
    <td>ler e armazenar os dados da nota fiscal a partir de pdf's nativos</td>
    <td>poder gerenciar os gastos da empresa, assim, planejar as estratégias futuras</td>
    <td>Must</td>
    <td>8</td>
    <td>Concluído</td>
  </tr>
  <tr style="color:green">
    <th>US08</th>
    <td>Deletar nota fiscal</td>
    <td>administrador</td>
    <td>deletar uma nota fiscal já registrada</td>
    <td>apagar o registro de algum nota fiscal do sistema</td>
    <td>Must</td>
    <td>2</td>
    <td>Concluído</td>
  </tr>
  <tr style="color:green">
    <th>US09</th>
    <td>Visualizar nota fiscal</td>
    <td>administrador ou funcionário</td>
    <td>visualizar dados de uma nota fiscal específica</td>
    <td>ter conhecimento dos gastos registrados em uma nota fiscal</td>
    <td>Must</td>
    <td>5</td>
    <td>Concluído</td>
  </tr>
  <tr style="color:green">
    <th>US10</th>
    <td>Listar nota fiscal</td>
    <td>administrador ou funcionário</td>
    <td>listar notas fiscais registradas no sistema</td>
    <td>ter conhecimento das notas fiscais registradas no sistema</td>
    <td>Must</td>
    <td>3</td>
    <td>Concluído</td>
  </tr>
  <tr style="color:green">
    <td rowspan="2">FE03 - Manuntenção das análises</td>
    <th style="color:red">US11</th>
    <td style="color:red">Selecionar análise</td>
    <td style="color:red">administrador ou funcionário</td>
    <td style="color:red">selecionar uma opção de análise financeira</td>
    <td style="color:red">ter uma visão de negócio mais ampliada a partir de vários tipos de análises</td>
    <td style="color:red">Must</td>
    <td style="color:red">13</td>
    <td style="color:red">Removido</td>
  </tr>
  <tr style="color:green">
    <th style="color:red">US12</th>
    <td style="color:red">Visualizar análise</td>
    <td style="color:red">administrador ou funcionário</td>
    <td style="color:red">visualizar detalhadamente uma análise específica</td>
    <td style="color:red">para ter conhecimento da análise dos gastos de um determinado período de tempo</td>
    <td style="color:red">Must</td>
    <td style="color:red">8</td>
    <td style="color:red">Removido</td>
  </tr>
  <tr style="color:green">
    <td rowspan="3"  style="color:green">FE09 - Dashboard</td>
    <th>US17</th>
    <td>Gráfico por valor e tempo</td>
    <td>administrador ou funcionário</td>
    <td>selecionar uma opção de análise financeira</td>
    <td>ter uma visão de negócio mais ampla a partir da análise do valor gasto pelo tempo</td>
    <td>Must</td>
    <td>8</td>
    <td>Concluído</td>
  </tr>
  <tr style="color:green">
    <th>US19</th>
    <td>Gráfico por categoria e valor</td>
    <td>administrador ou funcionário</td>
    <td>selecionar uma opção de análise financeira</td>
    <td>ter uma visão de negócio mais ampla a partir da análise do valor gasto pela categoria do gasto</td>
    <td>Must</td>
    <td>1</td>
    <td>Concluído</td>
  </tr>
  <tr style="color:green">
    <th>US20</th>
    <td>Gráfico por destinatario e valor</td>
    <td>administrador ou funcionário</td>
    <td>selecionar uma opção de análise financeira</td>
    <td>ter uma visão de negócio mais ampla a partir da análise do valor gasto por destinatario</td>
    <td>Must</td>
    <td>1</td>
    <td>Pendente</td>
  </tr>
</table>

## Technical Stories

Abaixo está descrito as histórias técnicas:

<table border="2">
  <tr>
    <th>ÉPICO</th>
    <th>FEATURE</th>
    <th>TS</th>
    <th>FUNCIONALIDADE</th>
    <th>EU, COMO...</th>
    <th>DESEJO...</th>
    <th>PARA...</th>
    <th>PRIORIDADE</th>
    <th>PONTUAÇÃO</th>
    <th>STATUS</th>
  </tr>
   <tr style="color:lime">
    <td rowspan="4">EP01 - Usuário</td>
    <td rowspan="1">FE04 - Sessão</td>
    <th>TS10</th>
    <td>Implementar API Gateway</td>
    <td>Desenvolvedor</td>
    <td>implementar a autenticação através do API Gateway</td>
    <td>criar a camada de segurança entre o micro serviço do front e os micro serviços do back end</td>
    <td>Should</td>
    <td >5</td>
    <td >Adicionada</td>
  </tr>
  <tr style="color:lime">
    <td rowspan="2">FE01 - Manuntenção do Funcionário</td>
    <th>TS12</th>
    <td>Popular banco de dados com funcionários e administrador </td>
    <td>Desenvolvedor</td>
    <td>popular o banco com registros</td>
    <td>verificar funcionamento do software em uso</td>
    <td>Must</td>
    <td >3</td>
    <td >Adicionada</td>
  </tr>
   <tr style="color:lime">
    <th>TS14</th>
    <td>Popular banco de dados com notas fiscais </td>
    <td>Desenvolvedor</td>
    <td>popular o banco com registros</td>
    <td>verificar funcionamento do software em uso</td>
    <td>Must</td>
    <td >8</td>
    <td >Adicionada</td>
  </tr>
  <tr style="color:lime">
   <td rowspan="1">FE08 - Instalação</td>
    <th>TS13</th>
    <td>Atualizar microserviços para build</td>
    <td>Desenvolvedor</td>
    <td>Alterar implementação de views e urls das aplicações</td>
    <td>ser possivel o build com pyinstaller</td>
    <td>Must</td>
    <td >13</td>
    <td >Adicionada</td>
  </tr>
  <tr style="color:green">
    <td rowspan="9">EP02 - Financeiro</td>
    <td rowspan="9">FE06 - Leitura da Nota Fiscal</td>
    <th>TS01</th>
    <td>Converter PDF</td>
    <td>Desenvolvedor</td>
    <td>converter o pdf de nota fiscal em texto</td>
    <td>o parser realizar a análise</td>
    <td>Must</td>
    <td>1</td>
    <td>Concluído</td>
  </tr>
  <tr style="color:green">
    <th>TS02</th>
    <td>Parser de nota fiscal</td>
    <td>Desenvolvedor</td>
    <td>realizar a análise sintática de cada nota fiscal</td>
    <td>poder criar uma estrutura de dados de notas fiscais</td>
    <td>Must</td>
    <td>21</td>
    <td>Concluído</td>
  </tr>
  <tr style="color:green">
    <th>TS07</th>
    <td>Refatorar parser (valor de imposto)</td>
    <td>Desenvolvedor</td>
    <td>refatorar a parte de imposto do parser da nota fiscal</td>
    <td>o sistema conseguir interpretar os dados de impostos adequadamente</td>
    <td>Must</td>
    <td>13</td>
    <td>Adicionada</td>
  </tr>
  <tr style="color:lime">
    <th>TS08</th>
    <td>Mudar conversor de PDF nativo</td>
    <td>Desenvolvedor</td>
    <td>mudar o conversor de pdf</td>
    <td> poder abranger uma maior quantidade de tipos de notas fiscais eletrônicas</td>
    <td>Must</td>
    <td>13</td>
    <td>Adicionada</td>
  </tr>
  <tr style="color:lime">
    <th>TS09</th>
    <td>Gerar novos gráficos a partir do Metabase</td>
    <td>Desenvolvedor</td>
    <td> gerar mais gráficos a partir dos dados das notas fiscais</td>
    <td> informar o usuário sobre o andamento dos gastos de sua empresa</td>
    <td>Should</td>
    <td>3</td>
    <td>Adicionada</td>
  </tr>
  <tr style="color:lime">
    <th>TS16</th>
    <td>Integrar Parser (Qt) com o PdfToInvoice (django rest) </td>
    <td>Desenvolvedor</td>
    <td>conectar o parser em qt com o back end em django rest</td>
    <td>o parser poder enviar os dados da nota fiscal lida para o banco de dados</td>
    <td>Must</td>
    <td>13</td>
    <td>Adicionada</td>
  </tr>
  <tr style="color:lime">
    <th>TS18</th>
    <td>Adicionar mydatabase ao repositório</td>
    <td>Desenvolvedor</td>
    <td>adicionar o arquivo mydatabase</td>
    <td>o metabase ter as migrations do banco de dados SQLite como base</td>
    <td>Must</td>
    <td>1</td>
    <td>Adicionada</td>
  </tr>
  <tr style="color:lime">
    <th>TS19</th>
    <td>Adicionar Autenticação no Worker Post</td>
    <td>Desenvolvedor</td>
    <td>implementar adicionar autenticação no Worker Post</td>
    <td>melhorar autenticação do sistema</td>
    <td>Must</td>
    <td>5</td>
    <td>Adicionada</td>
  </tr>
   <tr style="color:lime">
    <th>TS20</th>
    <td>Adicionar Autenticação em todas as páginas</td>
    <td>Desenvolvedor</td>
    <td>desejo só usuários logados possam acessar as páginas do sistema</td>
    <td>garantir a segurança do sistema</td>
    <td>Must</td>
    <td>8</td>
    <td>Adicionada</td>
  </tr>
  <tr style="color:green">
    <td rowspan="8">EP03 - Acessiblidade</td>
    <td rowspan="8">FE07 - Layout</td>
    <th>TS03</th>
    <td>Menu Lateral</td>
    <td>Desenvolvedor</td>
    <td>implementar layout do sistema</td>
    <td>dar acessibilidade ao usuário as funcionalidades existentes</td>
    <td>Must</td>
    <td>3</td>
    <td>Concluído</td>
  </tr>
  <tr style="color:green">
    <th>TS04</th>
    <td>Refatorar formulários</td>
    <td>Desenvolvedor</td>
    <td>refatorar formulários</td>
    <td>proporcionar uma interface mais acessível e padronizada</td>
    <td>Must</td>
    <td>3</td>
    <td>Adicionada</td>
  </tr>
  <tr style="color:green">
    <th>TS05</th>
    <td>Refatorar tabelas</td>
    <td>Desenvolvedor</td>
    <td>refatorar tabelas</td>
    <td>proporcionar uma interface mais acessível e padronizada</td>
    <td>Must</td>
    <td>3</td>
    <td>Adicionada</td>
  </tr>
  <tr style="color:green">
    <th>TS06</th>
    <td>Refatorar Menu Lateral</td>
    <td>Desenvolvedor</td>
    <td>refatorar menu lateral</td>
    <td>proporcionar uma interface mais acessível e padronizada</td>
    <td>Must</td>
    <td>3</td>
    <td>Adicionada</td>
  </tr>
  <tr style="color:lime">
    <th>TS11</th>
    <td>Adicionar gráficos nas páginas</td>
    <td>Desenvolvedor</td>
    <td>desejo disponibilizar os gráficos em páginas separadas</td>
    <td>detalhar mais os gastos da empresa</td>
    <td>Should</td>
    <td>5</td>
    <td>Adicionada</td>
  </tr>
   <tr style="color:lime">
    <th>TS15</th>
    <td>Refatorar código do front com ESlint</td>
    <td>Desenvolvedor</td>
    <td>refatorar código do front com ESlint</td>
    <td>adequar o código a nova folha de estilo do projeto</td>
    <td>Should</td>
    <td>5</td>
    <td>Adicionada</td>
  </tr>
  <tr style="color:lime">
    <th>TS17</th>
    <td>Implementar modal de criar Funcionário e Nota Fiscal</td>
    <td>Desenvolvedor</td>
    <td>implementar duas modais</td>
    <td>criar Funcionário e Nota Fiscal</td>
    <td>Must</td>
    <td>3</td>
    <td>Adicionada</td>
  </tr>
  <tr style="color:lime">
    <th>TS21</th>
    <td>Colocar layout fixo</td>
    <td>Desenvolvedor</td>
    <td> desejo deixar o menu lateral e superior fixo</td>
    <td>ter maior usabilidade ao rolar a página para baixo</td>
    <td>Should</td>
    <td>3</td>
    <td>Adicionada</td>
  </tr>
</table>
