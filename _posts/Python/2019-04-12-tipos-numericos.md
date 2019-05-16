---
title: Tipos Numéricos
published: true
tag: [Python]
categories: [Estudos]
---
## Como trabalhar com valores grandes?

Dificil de ler

```python
1000000000
```

Facil de ler!
```python
1_000_000_000
```

## Ver tipo de nÚmero
```py
num = 42
type(num)
````

ou
```py
type(1)
```

Em ambos os casos a resposta é:

```py
<class 'int'>
```

## Operações com números

+ -> Soma simples
```py
num = 42
num + num
84
```

- -> Subtração simples
```py
num = 42
num - 2
40
```
* -> multiplicação simples
```py
num = 42
num * 2
84
```

/ -> divisão simples

```py
num = 42
num / 2
21
````

\*\* ->  Pontência

```py
num = 42
2**num
4398046511104
```

// -> parte inteira da divisão

```py
num = 42
num// 3
14
```

% -> resto da divisão

```py
num=42
num%3
0
```

### Outros operadores:
`num += 1` -> `num = num + 1`

`num -= 1` -> `num = num - 1`

`num *= 1` -> `num = num * 1`

`num /= 1` -> `num = num / 1`

`num ** = 2` -> `num = num ** 1`

## Tipo Inteiro

É um número inteiro, sem casas decimais.
```py
inteiro = 1
print(inteiro)
print(type(inteiro))
```

Resposta

```py
1
<class 'int'>
```

## Tipo Float

É um número decimal! Em Python usa-se *PONTO* para separar estes valores!

Se os número for separado por virgula será gerardo uma ***tupla***!!!

```py
valor = 1.33
print(valor)
print(type(valor))
```

Resposta

```py
1.33
<class 'float'>
```

É possivel fazer dupla atribuição:

```py
valor1, valor2 = 1.33, 1.55
print(valor1)
print(type(valor1))
print(valor2)
print(type(valor2))
```

Resposta

```python
1.33
<class 'float'>
1.55
<class 'float'>
```

É possível converter um ***float*** para um ***int***. Mas perde-se precisão. (a parte decimal tem que sumir)

```python
valor = 1.33
res = int(valor)
print(valor)
print(type(valor))
```

Resposta

```python
1
<class 'int'>
```

É possível converter um ***float*** para um ***int***. Mas perde-se precisão. (a parte decimal tem que sumir)

```python
num = 1
conv = float(num)
print(float(num))
print(type(valor))
```

Resposta

```python
1.ooooo
<class 'float'>
```

## Números complexos

```python
variavel = 5j
print(variavel)
print(type(variavel))
```

Resposta

```python
5j
<class 'complex'>
```

- 
