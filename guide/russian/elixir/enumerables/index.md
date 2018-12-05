---
title: Enumerables
localeTitle: перечислимый
---
## Перечисления (Enum)

В объектно-ориентированных языках программирования вы будете использовать «цикл» для повторения одного и того же действия над куском данных в Elixir, поскольку переменные неизменяемы. Невозможно создать трейдационный цикл, вместо этого Elixir и другие языки функционального программирования полагаться на рекурсию. С рекурсией вы будете выполнять одно и то же действие над каждым элементом в списке без необходимости изменять переменную. Библиотека Enum, созданная в Elixir, делает это легко.

## пример

Используя `Enum.map` вы можете запустить анонимную функцию (функцию, которая не находится внутри модуля), проходящую через каждый элемент в списке. Это выполняет ту же задачу, что и трейдационный цикл, без необходимости изменять переменную аккумулятора.

```elixir
iex> Enum.map([1, 2, 3], fn(x) -> x * 2 end) 
 [2, 4, 6] 
```

## Методы в модуле Enum

Модуль Enum имеет более 70 различных функций для использования в Enumerables, перечисление их всех здесь займет несколько страниц. Вместо этого давайте рассмотрим наиболее часто используемые функции в модуле Enum.

### Enum.map

`Enum.map` запускает анонимную или захваченную функцию над списком.

```elixir
iex> Enum.map([5, 10, 15, 20], fn(x) -> x * 2 end) 
 [10, 20, 30, 40] 
```

#### Дополнительная информация:

*   [elixir-lang.org | рекурсия](https://elixir-lang.org/getting-started/enumerables-and-streams.html)
*   [hexdocs | Enum](https://hexdocs.pm/elixir/Enum.html)