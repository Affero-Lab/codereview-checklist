# Checklist para o codereview 

#### Geral

* [ ] O código está de acordo com as convenções (Grunt, Maven Checkstyle) ?
* [ ] As alterações de artefatos no banco de dados estão versionadas (Migrate Liquibase)?
* [ ] Os testes automatizados estão executando com sucesso (Jasmine, Junit) ?
* [ ] O código está legível para humanos ?
* [ ] Há código redundante ou duplicado?
* [ ] O código está modularizado ?
* [ ] Há reimplementações de códigos que já foram resolvidos por bibliotecas consolidadas?
* [ ] Há logs ou códigos de debug que podem ser removidos?
* [ ] Há utilização de referências fixas (nomes de pastas, arquivos etc) ?


#### Lógica

* [ ] O código escrito apresenta a lógica de decisões corretas (De acordo com a especificação) ?
* [ ] Há loops infinitos?

#### Testes
* [ ] O código é testável? (Exemplo: verificar se há dependências ocultas, se é possível inicializar os objetos, se os frameworks de testes podem usar os métodos etc) ?
* [ ] Os testes existem e apresentam uma boa cobertura? (Exemplo: Há testes de borda?, A árvore de decisão está coberta?)
* [ ] As exceções foram testadas?


#### Segurança / Programação Defensiva

* [ ] O código está livre de estruturas de tamanho constante e funções para dados de tamanho dinâmico sem checagem.
* [ ] Nunca faça código mais complexo que o necessário. Complexidade alimenta bugs, incluindo problemas de segurança.
* [ ] Qualquer código é inseguro até  que se prove o contrário.
* [ ] Sempre espere que o mais improvável possa acontecer no fluxo do seu código.

#### Desempenho
