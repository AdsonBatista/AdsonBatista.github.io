---
title: Escopo de variável
published: true
tag: [Python]
categories: [Estudos]
---

Dois casos de escopo:

- Variáveis Globais

	São Globais ou seja seu escopo compreende todo o programa.

- Variáveis Locais

	São reconhecidas apenas no bloco onde foram declaradas, ou seja, seu escopo está limitado ao bloco onde foi declarada.

Em Python a "tipagem de variável" é dinamica ou seja não é necessário declarar o tipo da variável, isto é feito de forma automática!

Re-atribuição é possivel, ou seja, é trocar o tipo de dado de uma variavel.

```Python
numero = 23
print(numero)
print(type(numero))

numero = 'Adson'
print(numero)
print(type(numero))
```

No exemplo acima `numero` é uma variável global ou seja pode ser usada em todo programa! 
Veja o exemplo abaixo.

```python
numero = 2
if numero >10:
    novo = numero + 1o
    print(novo)
    
print(novo)
```

Note que um erro irá aparecer pois a variável `novo`está declarada dentro do `if`, ou seja, ela é uma variável local válida apenas dentro do if. NOTA: Neste caso caso a condição do `if` seja válida a variável `novo`será impressa no terminal.