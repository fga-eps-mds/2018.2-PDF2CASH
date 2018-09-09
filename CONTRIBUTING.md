# Contribuindo com o PDF2CA$H.
***
Agredecemos sua vontade em contribuir com nosso projeto. A seguir encontram-se algumas diretrizes para aqueles que desejam realizar contribuições junto ao PDF2CA$H.

## Código de conduta

Ajude-nos a manter o bom convivio de nossa comunidade ao ler e seguir o nosso [código de conduta](/CODE_OF_CONDUCT.md).

## Como contribuir
***
### Reportando _bugs_
Caso tenha descoberto um _bug_ e deseja fazer um _report_ do mesmo por favor submita uma _issue_ seguindo este [template](.github/ISSUE_TEMPLATE/bug_report.md).
### Sugerindo melhorias
Caso tenha sugestões de melhorias ou deseja fazer um pedido de uma nova _feature_ por favor submita uma _issue_ seguindo este [template](.github/ISSUE_TEMPLATE/feature_request.md).
### _Pull Requests_
  * Preencha este [template](/PULL_REQUEST_TEMPLATE.md).
  * Siga o nosso [guia de estilo]().

## Guia de estilo
TODO / TBD
### Mensagens do git
  * Sempre use o infinitivo.
  * Usar o inglês.

  Certo:
  > Add new filter.

  Errado:
  > Adding new feature.

  * <a name="line-rule"></a>A primeira linha da mensagem deve ter no máximo 72 caracteres.

  * Use a primeira linha para fazer uma descrição sucinta da mudança proposta do commit. Use as linhas restantes para fazer uma descrição mais detalhas se for preciso.

  * Caso a mudança proposta no commit estiver relacionada à alguma issue favor  incluir uma indicação do mesmo da seguinte forma:
  > refs #<ISSUE_NUMBER>
  > refs #<ISSUE_NUMBER>, #<ISSUE_NUMBER>, ...

  A localização de tal indicação deve ser escolhida segundo as seguintes regras:
    * Caso o titulo do _commit_(e.g. primeira linha) suporte a inserção da indicação sem quebrar a regra de [72 caracteres](#line-rule), coloque um ';' ao final da mensagem seguido da indicação. Ex:

   > Fix a bug in the person's crud; refs #16

   * Caso contrário use uma linha separada para colocar a indicação. Ex:

   > Implement the search algorithm for cases in which the input is greather than 20

   > refs: #15, #17.
