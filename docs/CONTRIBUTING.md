# Contribuindo com o PDF2K-Nativo.
***
Agredecemos sua vontade em contribuir com nosso projeto. A seguir encontram-se algumas diretrizes para aqueles que desejam realizar contribuições junto ao _PDF2K_-Nativo.

## Código de conduta

Ajude-nos a manter o bom convivio de nossa comunidade ao ler e seguir o nosso [código de conduta](/docs/CODE_OF_CONDUCT.md).

## Como contribuir
***
### Reportando _bugs_
Caso tenha descoberto um _bug_ e deseja fazer um _report_ do mesmo por favor submita uma _issue_ seguindo este [template](/docs/ISSUE_TEMPLATE/BUG_ISSUE_TEMPLATE.md).
### Sugerindo melhorias
Caso tenha sugestões de melhorias ou deseja fazer um pedido de uma nova _feature_ por favor submita uma _issue_ seguindo este [template](/docs/ISSUE_TEMPLATE/FEATURE_ISSUE_TEMPLATE.md).
### _Pull Requests_
  * Preencha este [template](/docs/PULL_REQUEST_TEMPLATE.md).
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

  * A primeira linha da mensagem deve ter no máximo 72 caracteres.

  * <a name="line-rule"></a> Use a primeira linha para fazer uma descrição sucinta da mudança proposta do commit. Use as linhas restantes para fazer uma descrição mais detalhas se for preciso.

  * Se for apenas uma nova documentação, adicione [ci skip] no titulo do commit.

  * Caso a mudança proposta no commit estiver ligada á alguma issue favor  incluir uma indicação do mesmo da seguinte forma:
  > closes #<ISSUE_NUMBER>

  A localização de tal indicação deve ser escolhida segundo as seguintes regras:
    * Caso o titulo do _commit_(e.g. primeira linha) suporte a inserção da indicação sem quebrar a regra de [72 caracteres](#line-rule), coloque um ';' ao final da mensagem seguido da indicação. Ex:
    > Fix a bug in the person's crud; closes \#16

    * Caso contrário use uma linha separada para colocar a indicação. Ex:
    > Implement the search algorithm for cases in which the input is greather than 20

     > closes: \#15,\#17.
