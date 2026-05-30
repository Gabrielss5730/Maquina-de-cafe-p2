# Maquina-de-cafe-p2
# Avaliação P2 - Linguagem de Programação - Prof. Bruno Zolotareff

## Integrantes

- Gabriel Silva

## Sobre o Projeto

Este projeto foi desenvolvido em Java com o objetivo de simular o funcionamento de uma máquina de café com seis sabores disponíveis. O usuário pode acessar um menu, escolher a bebida desejada e acompanhar a simulação do preparo.

Para o desenvolvimento da aplicação foram utilizados conceitos de Programação Orientada a Objetos (POO), incluindo uma classe abstrata chamada `Drink`, uma classe concreta chamada `Cafe` e uma classe principal responsável pela execução do sistema.

---

## Conceitos de Programação Orientada a Objetos Aplicados

### Abstração

A abstração foi aplicada através da classe abstrata `Drink`. Ela representa uma bebida de forma genérica, reunindo atributos e métodos que podem ser compartilhados por todas as bebidas da aplicação.

Dessa forma, a classe serve como um modelo para as demais classes, sem precisar definir todos os detalhes de funcionamento.

### Herança

A herança foi utilizada quando a classe `Cafe` herdou as características da classe `Drink`.

Com isso, foi possível reaproveitar atributos e métodos já existentes, evitando repetição de código e tornando a estrutura do sistema mais organizada.

### Encapsulamento

O encapsulamento foi aplicado protegendo os atributos das classes por meio de modificadores de acesso e utilizando métodos getters e setters para controlar o acesso aos dados.

Esse conceito aumenta a segurança e a organização do código, garantindo que as informações sejam manipuladas de forma adequada.

---

## Aplicação do Polimorfismo

O polimorfismo permite que objetos diferentes sejam tratados através de uma mesma referência da classe pai.

Na máquina de café, além da classe `Cafe`, poderiam existir outras classes como `Capuccino`, `ChocolateQuente` e `Mocha`, todas herdando de `Drink`.

Assim, uma variável do tipo `Drink` poderia armazenar qualquer uma dessas bebidas:

```java
Drink bebida = new Cafe();
bebida.preparar();

bebida = new Capuccino();
bebida.preparar();
```