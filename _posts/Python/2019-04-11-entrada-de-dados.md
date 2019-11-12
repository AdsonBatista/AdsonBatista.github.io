---
title: Recebendo dados do usuário!
tag: [Python]
categories: [Estudos]
categories: [Estudos]
---

A entrada de dados é feita com o comando `input()`. Todo "dado" recebido por este comando é do tipo ***String***.

***String*** em **Python** é tudo que estiver entre:
- Aspas simples; -> 'Adson Batista'
- Aspas duplas; -> "Adson Batista"
- Aspas simples triplas -> '''Adson Batista'''
- Aspas duplas triplas -> """Adson Batista"""

# Exemplos de interações com entrada de dados

## Uma única entrada textual.

- Perguntar qual é o nome de uma pessoa:
    
    ```pyton
    print("Qual seu nome? ")
    nome = input()
    ```
- Reescrevendo o a pergunta anterior:

    ```python
    nome = input("Qual seu nome? ")
    ```

### Respondendo utilizando a variável de entrada:

- Exemplo de resposta utilizando o *print* da versão 2.x

```python
print("Seja vem vindo(a) %s" % nome)
```

- Exemplo de resposta utilizando o *print* da versão 3.x

```python
print('Seja bem vindo(a) {0}'.format(nome))
```

- Exemplo de resposta utilizando o *print* da versão 3.7

```python
print(f'Seja vem vindo(a) {nome}')
```

## Duas entradas de dados uma textual e outra numérica.

```python
nome = input("Qual seu nome? ")
print(f'Seja vem vindo(a) {nome}')
idade = input("Qual sua idade? ")
```    

### Utilizando variáveis no texto


#### uma variável

- Exemplo de resposta utilizando o *print* da versão 2.x

```python
print("Seja vem vindo(a) %s" % nome)
```

- Exemplo de resposta utilizando o *print* da versão 3.x

```python
print('Seja bem vindo(a) {0}'.format(nome))
```

- Exemplo de resposta utilizando o *print* da versão 3.7

```python
print(f'Seja vem vindo(a) {nome}')
```

#### Duas variáveis

- Exemplo de resposta utilizando o *print* da versão 2.x

```python
# print("A %s tem %s anos" % (nome,idade))
```

- Exemplo de resposta utilizando o *print* da versão 3.x

```python
# print("A {0} tem {1} anos".format(nome,idade))
```

- Exemplo de resposta utilizando o *print* da versão 3.7

```python
print(f'A {nome} tem {idade} anos')
```

## Conversão de tipo de  dados ***Cast***

***Cast*** é a conversão de um tipo de dados para outro

```python
int(string)
```

O ***Cast*** pode ser feito na entrada de dados!!

```python
idade = int(input("Qual sua idade? "))
print(f'A {nome} nasceu em {2019 - idade}')
```

## Manipulando a variáveis dentro de um texto

```python
print(f'A {nome} nasceu em {2019 - int(idade)}')
```
