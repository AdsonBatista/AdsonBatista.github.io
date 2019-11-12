---
title: Tipo string
published: true
tag: [Python]
categories: [Estudos]
---

Em Python, um dado é considerado do tipo String sempre que estiver entre:

- Aspas simples :

  ```python
  'uma string', '2313', 'a', 'True'
  ```

- Duplas :

  ```python
  "uma string", "2313", "a","True"
  ```

- Triplas:

  ```python
  '''uma string''', '''2313''', '''a''', '''True'''
  ```

- Tres aspas duplas:

  ```python
  """uma string""", """2313""", """a""","""'True"""	
  ```

O mais comum é utilizar aspas simples! Mas as vezes é necessário utilizar os outros tipos.

- Quebra de linha:

```python
print('Adson \nBatista')
```

Resposta:

```python
Adson 
Batista
```

- Todo texto em caixa alta

  ```python
  nome = 'Adson Batista'
  print(nome.upper())
  ```

   Resposta: 

  ```python
  ADSON BATISTA
  ```

  

- Todo texto em caixa baixa

- ```python
  nome = 'Adson Batista'
  print(nome.lower())
  ```
   Resposta: 

  ```python
  adson batista
  ```

- Separar palavras em uma lista de strings

  ```python
  nome = 'Adson Batista'
  print(nome.split())
  ```
  Resposta: 

  ```python
  ['Adson', 'Batista']
  ```


  - Imprimir determinada palavra:

  ```python
nome = 'Adson Batista'
print(nome.split()[0])
  ```

  Resposta: 

  ```python
Adson
  ```

## Caracteristica importante

Em Python uma string é uma lista de letras por definição! Para acessar posição da lista (slice de string). A contagem de posicição de uma lista inicia em ZERO. No print a posição inicial é incluída na impressão e a ultima posição é excluída.

  ```python
nome = 'Adson Batista'
print(nome[0:5])
  ```

​	Resposta

  ```Python
Adson
  ```

- Inverter uma String completa:

    ```
    nome = 'Adson Batista'
    print(nome[::-1])
    ```

  Resposta:

    ```
  atsitaB nosdA
    ```

-  Substituir Letras (replace('original'.'nova'))

  ```python
  nome = 'Adson Batista'
  print(nome.replace('a','c'))
  ```

  Resposta:

  ```python
  Adson Bctistc
  ```

  

