---
title: Tipo Booleano
published: true
tag: [Python]
categories: [Estudos]
---

Existem duas constantes: ***True*** para Verdadeiro e ***False*** para falso. SEMPRE com as iniciais maiúsculas.

- ***True***

  ```py
  ativo = True
  print(ativo)
  ```

  Resposta:

  ```py
  True
  ```

- ***False***

  ```py
  ativo = False
  print(ativo)
  ```

  Resposta:

  ```py
  False
  ```

## Operações booleanas

- Negação (`not`)

  Nega o valor atual, se o valor for verdadeiro a resposta será falsa ou se o valor for falso a resposta será verdadeira

  ```
  ​```py
  ativo = True
  print(not ativo)
  ​```
  
  resposta
  
  ​```py
  False
  ​``` 
  ```

- Ou (`or`)

  É uma operação binária. Depende de dois valores. Se pelo menos um dos valores for verdadeiro a operação é verdadeira.

  `True or True` -> `True`
  `True or False` -> `True`
  `False or True` -> `True`
  `False or False` -> `True`

- E (`and`)

  É uma operação binária, ou seja, depende de dois valores. Se ambos os valores forem verdadeiros ela é verdadeira. caso contrário é falsa.

  `True and True` -> `True`
  `True and False` -> `False`
  `False and True` -> `False`
  `False and False` -> `False`

- Comparadores 

  - Maior (>) -> `num1 > num2`
  - Maior (>=) -> `num1 >= num2`
  - Menor (<) -> `num1 < num2`
  - Menor ou igual (<=) -> `num1 <= num2`
  - Igual (==) -> `num1 == num2`

- Combinando
  - or

    ```python
    num1 = 1
    num2 = 2
    num1 < num2 or num1>3
    ```
    Resposta:

    ```python
    True
    ```

  - and

    ```py
    num1 = 1
    num2 = 2
    num1 < num2 and num1>3
    ```

    Resposta:

    ```py
    False
    ```

  

