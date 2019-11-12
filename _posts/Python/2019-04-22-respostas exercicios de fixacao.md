---
title: Respostas Exercicios de Fixação
published: true
tag: [Python]
categories: [Estudos]
---

1. Faça um programa que leia um número inteiro e o imprima.
    ```python
    num = int(input('Entre com um número inteiro: '))
    print(f'O numero inteiro que você digitou foi: {num}')
    ```
2. Faça um programa que leia um número real e o imprima.
    ```python
    num = float(input('Entre com um número decimal: '))
    print(f'O número decimal que você entrou foi: {num}')
    ```

3. Peça ao usuário para digitar três valores inteiros e imprima a soma deles.
    ```python
    num1 = float(input("Digite um número real: "))
    num2 = float(input("Digite outro número real: "))
    num3 = float(input("Digite mais um número real: "))
    print(f'A soma dos números digitados é: {num1 + num2 + num3}')
    ```

4. Leia um número real e imprima o resultado do quadrado desse número.
    ```python
    num = float(input('Digite um número real: '))
    print(f'O quadrado do número digitado é {num**2}')
    ```

5. Leia um número real e imprima a quinta parte deste número.
    ```python
    num = float(input("Digite um número real: "))
    quintaparte = num/5
    print(f'A quinta parte do número digitado é {quintaparte}')
    ```

6. Leia uma temperatura em graus Celsius e apresente-a convertida em graus Fahrenheit. A fórmula de conversão é: C=5.0*(F-32.0)/9.0, sendo F a temperatura em Fahrenheit e C a temperatura em Celsius.
    ```python
    temp_ceulsius= float(input('Qual a temperatura em Graus Celsius? '))
    temp_fahrenheit= temp_ceulsius*9/5+32
    print("A temperatura em Fahrenheit é de %s" %temp_fahrenheit)
    ```

7. Leia uma temperatura em graus Fahrenhhiet e apresente-a convertida em graus Celsius.
    ```python
    temp_fahrenheit = float(input('Qual a temperatura em Graus Fahrenheit? '))
    temp_ceulsius = 5.0*(temp_fahrenheit-32)/9.0
    print("A temperatura em ceulsius é de %s" %temp_ceulsius)

    ```


8. Leia uma temperatura em Kelvin e apresente-a convertida em graus Celsius. A formula de conversão é: C = K-273.15
    ```python
    temp_kelvin = float(input("Temperatura em Kelvin: "))
    temp_celsius = temp_kelvin - 273.15
    print('A temperatura é de %s graus Celsius' %temp_celsius)
    ```

9. Leia uma temperatura em graus Celsius e apresente-a convertida em Kelvin.
    ```python
    temp_celsius = float(input('Temperatuda em graus Celsius '))
    temp_kelvin = temp_celsius + 273.15
    print(f'A temperatura em Kelvin é {temp_kelvin}')
    ```

10. Leia uma velocidade em km/h e apresente-a convertida em m/s.
    ```python
    velocidade_kmh=float(input('Qual a velocidade em km/h? '))
    velocidade_ms=velocidade_kmh / 3.6
    print(f'A velocidade em m/s é de {velocidade_ms}')
    ```

11. Leia uma velocidade em m/s e apresente-a convertida em km/h
    ```python
    velocidade_ms = float(input('Qual a velocidade em m/s? '))
    velocidade_kh = velocidade_ms * 3.6
    print(f'A velocidade em Km/h é de {velocidade_kh}')
    ```

12. Leia uma distância em milhas e apresente-a convertida em quilômetros.
    ```python
    distancia_milhas = float(input('Qual a distância em milhas? '))
    distancia_km = distancia_milhas * 1.609344
    print(f'A distância em Km é de {distancia_km}.')
    ```

13. Leia uma distância em quiômetros e apresente-a convertida em milhas.
    ```python
    distancia_km = float(input('Qual a distância em km? '))
    distancia_milhas = distancia_km / 1.609344
    print(f"A distancia em milhas é {distancia_milhas}")
    ```

14. Leia um ângulo em graus e apresente-o convertido em radianos.
    ```python
    ang_graus = float(input("Entre com ângulo em graus "))
    ang_rad = ang_graus * 0.01745
    print(f'O ângulo em radianos é {ang_rad}')
    ```

15. Leia um ângulo em radianos e apresente-o convertido em graus.
    ```python
    angulo_rad = float(input("Digite o valor do angulo em radianos: "))
    angulo_graus = angulo_rad / 0.01745
    print(f"O valor do angulo em graus é: {angulo_graus}")
    ```

16. Leia um vlaor de comprimento em polegadas e apresente-o convertido em centímetros. 
    ```python
    comprimento_pol = float(input("Digite o valor do comprimento em polegadas: "))
    comprimento_cm = comprimento_pol * 2.54
    print(f'O comprimento em cm é: {comprimento_cm}')
    ```

17. Leia um valor de comprimento em centímetros e apresente-o convertido em polegadas.
    ```python
    comprimento_cm = float(input("Digite o comprimento em cm: "))
    comprimento_pol = comprimento_cm / 2.54
    print(f"O comprimento em polegadas é: {comprimento_pol}")
    ```

18. Leia um valor de volume em metros cúbicos e apresente-o convertido em Litros
    ```python
    volume_mcubi = float(input("Entre com valor do volume em metros cubicos: "))
    volume_litros = volume_mcubi * 1000
    print(f"O volume em litros é: {volume_litros}")
    ```

19. Leia um valor em Litros e apresente-o convertido em metros cúbicos.
    ```python
    volume_litros = float(input("Digite o volume em litros: "))
    volume_mcub = volume_litros /1000
    print(f"O volume em metros cubicos é: {volume_mcub}")
    ```

20. Leia um valor de massa em quilogramas e apresente-o convertido em libras.
    ```python
    massa_kg = float(input('digite o valor da massa em kg: '))
    massa_libras = massa_kg * 2.205
    print(f"O valor da massa em libras é de: {massa_libras}")
    ```

21. Leia um valor de massa em libras e apresente-o convertido em quilogramas.
22. Leia um valor de comprimento em jardas e apresente-o convertido em metros
23. Leia um valor de comprimento em metros e apresente-o convertido em jardas.
24. Leia um valor de área em metros quadrados e apresente-o convertido em acres.
25. Leia um valor de área em acres e apresente-o convertido em metros quadrados.
26. Leia um valor de área em metros quadrados e apresente-o convertido em hectares.
27. Leia um valor de área em hectares e apresente-o convertido em metros quadrados.
28. Faça a leitura de três valores e apresente como resultado a soma dos quadrados dos três valores lidos.
29. Leia quatro notas, calcule a média aritmética e imprima o resultado.
30. Leia um valor em real e a cotação do dólar. Em seguida, imprima o valor correspondente em dólares.
31. Leia um número inteiro e imprima o seu antecessor e seu sucessor.
32. Leia um número inteiro e imprima a soma do sucessor e do seu triplo com o antecessor de seu dobro.
33. Leia o tamanho do lado de um quadrado e imprima como resultado a sua área.
34. Leia o valor do raio de um circulo e calcule e imprima a área do circulo correspondente.  Pi = 3.141592
35. Sejam a e b os catetos de um triângulo, onde a hipotenusa é obtida pela equação: hipotenusa = raiz quadrada da soma do quadrado dos catetos. Faça um programa que receba os valores de a e b e calcule o valor da hipotenusa através da equação. Imprima o resultado dessa operação.
36. Leia a altura e o raio de um cilindro circular e imprima o volume do cilindro. 
37. Faça um programa que leia o valor de um produto e impirma o valor com desconto, tendo em vista que o desconto foi de 12%.
38. Leia o salário de um funcionário. Calcule e imprima o valor do novo salário, sabendo que ele recebeu um aumento de 25%.
39. A importância de R$780.000,00 será dividida entre três ganhadores de um concurso. Sendo que a quantida total:
	- O primeiro ganhador receberá 46%;
	- O segundo receberá 32%;
	- O terceiro ganhará o restante;
	Calcule e imprima a quantia ganha por cada um dos ganhadores.
40. Uma empresa contrata um encanador a R$30,00 por dia. Faça um programa que solicite o número de dias trabalhados pelo encanador e imprima a quantia liquida que deverá ser paga, sabendo-se que são descontados *% para o imposto de renda.
41. Facá um programa que leia o valor da hora de trabalho (em reais) e o número de horas trabalhadas no mês. Imprima o valor a ser pago ao funcionário, adicionando 10% sobre o valor calculado.
42. EReceba o salário-base de um funcionário. Calcule e imprima o salário a receber, sabendo-se que esse funcionário tem uma gratificação de 5% sobre o salário-base. Além disso ele paga 7% de imposto sobre o salário-base.
43. Escreva um programa de ajuda para vendedores. A partir de um valor total lido, mostre:
	- .O total a pagar com desconto de 10%
	- O valor de cada parcela, no parcelamento de 3x sem juros
	- a comissão do vendedor, no caso da venda ser a vista (5% sobre o valor com desconto)
	- a comissão do vendedor, no caso da venda ser parcelada (5% sobre o valor total)
44.  Receba a altura do degrau de uma escada e a altura que o usuário deseja alcançar subindo a escada. Calcule e mostre quantos degraus o usuário deverá subir para atingir seu objetivo.
45.  Faça um programa para converter uma letra maiúscula em letra minúscula. Use a tabela ASCII para resolver o problema.
46.  Faça um programa que leia um número inteiro positivo de três digitos (de 100 a 999). Gere outro número dormado pelos dígitos invertidos do número lido.
47.  Leia um número inteiro de 4 dígitos (de 1000 a 9999) e imprima 1 dígito por linha.
48.  Leia um valor inteiro em segundos, e imprima-o em horas, minutos e segundos.
49.  Faça um programa para ler o horário (hora, minuto e segundo) de inicio e a duração em segundos, de uma experiência biológica. O programa deve resultar com novo horário (hora, minuto e segundo) do termino da mesma.
50.  Implemente um programa que calcule o ano de nascimento de uma pessoa a partir de sua idade e do ano atual.
51.  Escreva um programa que leia as coordenadas x e y de pontos no Rˆ2 e calcule sua distância da origem (0,0)
52.  Três amigos jogaram na loteria. Caso eles ganhem o prêmio deve ser repartido proporcionalmente ao valor que cada deu para realização da aposta. Faça um programa que leia quanto cada apostador investiu, o valor do prêmio e imprima quanto cada um ganharia do prêmio com base no valor investido.
53.  Faça um programa para ler as dimensões de um terreno (comprimento e largura) bem como o preço do metro de tela. Imprima o custo para a cercar este mesmo terreno com tela. 
