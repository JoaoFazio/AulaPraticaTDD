# Aula Prática de TDD

Repositório com o exercício prático de TDD (Test-Driven Development), baseado no clássico exemplo do livro do Kent Beck, reproduzido conforme o roteiro do Prof. Marco Tulio Valente (UFMG).

## Sobre o exercício

O objetivo foi implementar, através do ciclo **vermelho → verde → refactor**, um sistema de representação monetária (`Money`) capaz de lidar com múltiplas moedas (dólares e francos suíços), aplicando testes unitários com JUnit a cada passo.

## Tecnologias

- Java 17
- Maven
- JUnit 4

## Estrutura final

O código evoluiu de duas classes concretas (`Dollar` e `Franc`) para uma única classe `Money`, unificada através de sucessivos refactors — eliminando duplicação e usando métodos fábrica (`Money.dollar(...)`, `Money.franc(...)`) para criação de instâncias.

- `src/main/java/org/example/Money.java` — implementação final
- `src/test/java/org/example/DollarTest.java` — suíte de testes

## Como rodar os testes

```bash
mvn test
```

## Roteiro original

https://github.com/mtov/AulaPraticaTDD
