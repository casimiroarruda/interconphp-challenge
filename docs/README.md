Intercon PHP
===

Especificação
---

### Objetivo

Uma aplicação simples feita em diferentes frameworks. Essa é a ideia principal. A aplicação em questão é uma lista
 de tarefas a fazer, um TO-DO. O principal é mostrar como os frameworks trabalham para te ajudar em um projeto.
 
### Aplicação

#### Tarefa

Uma tarefa é composta por pelo menos 4 atributos como no "Diagrama" a seguir:

|Task        |
______________
|id          |
______________
|title       |
 _____________
|description |
______________
|status      |
______________

Vocês estão livres para decidir sobre os tipos desses atributos e se os mesmos são suficientes para realizar a tarefa.
 O importante é que pelo menos estes campos sejam mantidos para comparação entre o projeto em cada framework

#### Lista

Listar as tarefas já adicionadas. Ao clicar em uma ela ganha o status de *Done*. As tarefas com status *Done* ficam 
  na parte de baixo da lista enquanto que as que não tiverem esse status ficam no topo; neste momento não se faz 
  necessário uma confirmação para marcá-la como *Done*.
  
A exibição de uma tarefa consiste em seu título basicamente. Sua descrição deve ser exibida via tooltip ou outro auxílio 
  visual compatível.
  
#### Adição de novas tarefas

Ao acionar o gatilho de nova tarefa (no layout proposto um botão com **+**) uma nova atividade (representada pelo 
 componente paper-dialog no layout proposto) deve exibir um formulário para adição de nova tarefa, com entradas para os 
 campos de título e descrição 

Ao acionar o gatilho de persistência (representado pelo botão *Salvar* no layout proposto) esses dados devem ser 
 persistidos, a atividade de adição ocultada ou encerrada, e a atividade principal ser atualizada de maneira que a nova
 tarefa seja exibida.

#### Atividades

Por atividade entenda-se escopo de interação da aplicação - página ou formulário. Em nossa aplicação temos basicamente 
 duas:
 
* Lista (a atividade principal)
* Formulário de adição.

#### Arquitetura

Vocês estão livres para decidir fazer uma aplicação tradicional, com substituição de variáveis e lógica no template ou
 se quiserem fazer um webservice para ser consumido via javascript.

O importante é mostrar como o seu framework pode resolver melhor o problema :)
