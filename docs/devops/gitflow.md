# Gitflow

## Objetivo

O presente documento tem como objetivo apresentar o modelo de fluxo de trabalho _git_ que os colaboradores do projeto PDF2CASH deverão seguir a fim de estarem de acordo com as necessidades exigidas pelo desenvolvimento ágil, bem como a integração/entrega contínua.

## Modelo de workflow

O modelo escolhido para satisfazer estas necessidades baseia-se fortemente nos famosos modelos [Github Flow](https://guides.github.com/introduction/flow/) e [Gitflow](https://nvie.com/posts/a-successful-git-branching-model/). De cada um foram retirados aspectos que foram tidos como pertinentes ao atual cenário de desenvolvimento. Um exemplo do modelo pode ser visualizado na seguinte figura:

![Gitflow model](/docs/assets/gitflow.png)

### _Branch_ de produção

É na _branch_ _Master_  onde o código 'pronto para produção' deverá residir. Isto quer dizer que o código só poderá ser enviado á _branch_ _Master_ quando estiver estável,válido e limpo. O _HEAD_ desta branch sempre deverá estar apontando para tag commits.

### _Branch_ de homologação

A branch de homologação utilizada pelo projeto será a _development_. Será nela onde deverá residir o código usado para gerar _builds_ para o ambiente de homologação/teste. Além disso é a partir da _development_ que _feature_ _branchs_ deverão ser criadas.

### _Branch_ de feature

As branchs de features serão utilizadas para o desenvolvimento de novas funcionalidades. Uma vez que a funcionalidade estiver completa, um pull request à _development_ deverá ser feito.

### _Branch_ de correção(hotfix)

Além das branchs usuais listadas acima, existem também as branchs de documentação e correção de bugs. As branchs de _hotfix_ servem como uma forma de correção de _bugs_ urgentes em produção. Consequentemente _hotfix_ branchs devem ser criadas a da última versão da branch _master_.

## Fluxos

### Fluxo padrão de desenvolvimento.

1. Inicia-se trabalho em uma nova _issue_.
2. Cria-se uma nova _feature_ branch a partir da _development_.
3. Criam-se modificações(commits).
4. Executam-se testes.
4. Ocorrendo tudo bem no passo anterior publica-se a branch para o remoto(origin).
5. Um _pull_ _request_ para a branch de homologação(_development_) deve ser feito e um revisor atribuído.
7. O revisor deve realizar uma análise das alterações propostas.
8. O revisor aceita o pull request caso seja válido ou notifica inconsistências encontradas por meio de comentários no _pull_ _request_.
9. A _feature_ _branch_ é integrada a _development_ e por meio do deploy contínuo enviada ao servidor de homologação.

### fluxo padrão de release

Assim que a branch de homologação(_development_) tiver acumulado mudanças válidas o suficiente que se adequem em uma nova versão de produção, deve-se fazer os preparativos para uma nova release. Para tanto deverá ser criada uma nova branch da _development_, uma _release_ _branch_, para que uma verificação final seja feita(limpeza, mudança de versão, etc...). Uma vez que a branch de _release_  estiver pronta, deverá ser integrada a _master_ por meio de um merge. Esta por sua vez deverá receber uma nova _tag_ e enviada ao servidor de produção via deploy contínuo.

## Convenção de nomes

A excessão das _branchs_ de produção e homologação que terão seus nomes fixos, as branchs de _features_,_releases_,_hotfix_ e documentação deverão seguir a seguinte convenção:

* Branch de _feature_
```
  feature/<feature_name>
  ex: feature/cv-parser
```

* Branch de _release_
```
  release/<release_version>
  ex: release/1.4
```
* Branch de _hotfix_
```
hotfix/<hotfix_version>
ex: hotfix/1.45
```

* Branch de documentação
```
documentation/<document_name>
ex: documentation/vision
```

Aplicam-se a todas as branchs acima:

* Escolha nomes curtos e descritivos.
* Os nomes das branchs devem ser em inglês.
* Em caso de nomes compostos, a separação das palavras deve ser via _hyphen_ _case_.
```
feature/create-filter
```


## Referências bibliográficas

1. https://nvie.com/posts/a-successful-git-branching-model/
2. https://guides.github.com/introduction/flow/
3. https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow
4. https://www.atlassian.com/continuous-delivery/continuous-delivery-workflows-with-feature-branching-and-gitflow
