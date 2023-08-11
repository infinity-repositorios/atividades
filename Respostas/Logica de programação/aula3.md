# Laços de Repetição:
## Questão 1:
~~~py
numMaior = 0

for i in range(3):
    num = float(input("Digite um numero qualquer: "))

    if num > numMaior:
        numMaior = num

print(f"O maior numero é igual a: {numMaior}")

print("=========================")

contador = 0
numMaior = 0

while contador < 3:
    num = float(input("Digite um numero qualquer: "))

    if num > numMaior:
        numMaior = num
    contador += 1

print(f"O maior numero é igual a: {numMaior}")
~~~
## Questão 2:
~~~py
num = int(input("Digite um numero de 1 a 10 para mostrar a tabuada de soma: "))

for i in range(1, 11):
    soma = num + i

    print(f"{num} + {i} = {soma}")

print("====================")

contador = 1

while contador <= 10:
    soma = num + contador

    print(f"{num} + {contador} = {soma}")

    contador += 1
~~~
## Questão 3:
~~~py
acumulado = 0

for i in range(5):
    num = float(input("Digite um numero qualquer: "))

    acumulado += num

media = acumulado / 5

print(f"A soma de todos os numeros foi: {acumulado}\n" +
f"E a media foi: {media}")

print("================")

acumulado = 0
contador = 0

while contador < 5:
    num = float(input("Digite um numero qualquer: "))

    acumulado += num

    contador += 1

media = acumulado / 5

print(f"A soma de todos os numeros foi: {acumulado}\n" +
f"E a media foi: {media}")
~~~
## Questão 4:
~~~py
acumulado = 0
contagem = 0
nota = 1

while nota != 0:
    nota = float(input("Digite a nota: "))

    if nota != 0: 
        acumulado += nota
        contagem += 1

media = acumulado / contagem

print(f"A media total das notas foi: {media}")
~~~
## Questão 5:
~~~py
contagem = 0

for i in range(10):
    num = int(input("Digite um numero qualquer: "))

    if 25 < num < 75:
        contagem += 1

print(f"O total de numeros entre 0 e 75 foram: {contagem}")

print("===================")

contagem = 0
contador = 0

while contador < 10:
    num = int(input("Digite um numero qualquer: "))

    if 25 < num < 75:
        contagem += 1
    
    contador += 1

print(f"O total de numeros entre 0 e 75 foram: {contagem}")
~~~
## Questão 6:
~~~py
for i in range(1, 11):

    for j in range(1, 11):
        mult = i * j

        print(f"{i} * {j} = {mult}")
    
    print("________________________________")

print("=============================")

x = 1
y = 1

while x <= 10:

    while y <= 10:
        mult = x * y

        print(f"{x} * {y} = {mult}")
        
        y += 1
    
    x += 1
    y = 1
    
    print("________________________________")
~~~
## desafio:
~~~py
tam = int(input("Digite o tamanho do triangulo: "))

lado = 1

for i in range(tam):
    
    for j in range(lado):
        print("*", end=" ")

    print()
    
    lado += 1

print("===============================")

lado = 1
x = 0
y = 0

while x < tam:

    while y < lado:
        print("*", end=" ")
        y += 1
    
    print()
    
    lado += 1
    y = 0
    x += 1
~~~

## Atividades lógica: <br>
https://github.com/infinity-repositorios/atividades/blob/main/guias/Lógica%20da%20Programação.md
## Menu:
https://github.com/infinity-repositorios/atividades