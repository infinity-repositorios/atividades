# Atividades aula 1

## Listas e Tuplas

## Questão 1

~~~py
lista_numerica = list()

for i in range(12):
    numero = int(input("Digite um numero qualquer: "))
    lista_numerica.append(numero)

print(lista_numerica)

x = int(input("Digite uma posição de 0 a 11: "))
y = int(input("Digite outro posição de 0 11: "))

soma = lista_numerica[x] + lista_numerica[y]

print(f"A soma das duas posições é: {soma}")
~~~

## Questão 2

~~~py
lista_impares = list()

while True:
    num = int(input("Digite um numero qualquer: "))

    if num % 2 != 0:
        lista_impares.append(num)

        if len(lista_impares) == 10:
            print(lista_impares)
            break
~~~

## Questão 3

~~~py
lista_numerica = list()

contador = 0

for i in range(10):
    numero = int(input("Digite um numero qualquer: "))

    lista_numerica.append(numero)

x = int(input("Digite um numero para verificar se exixte na lista: "))

for j in lista_numerica:
    if j == x:
        print(f"O numero: {x}, está na posição: {contador}")
        break
    contador += 1
else:
    if x not in lista_numerica:
        print("Numero não encontrado")
~~~

## Questão 4

~~~py
lista_numerica = list()

contador = 0

for i in range(20):
    num = int(input("Digite um valor qualquer positivo: "))

    lista_numerica.append(num)

for j in lista_numerica:

    if j % 2 == 0:
        contador += 1

print(contador)
~~~

## Questão 5

~~~py
lista_numero = list()

for i in range(20):
    num = int(input("Digite um numero positivo ou negativo: "))

    lista_numero.append(num)

for j in range(0, len(lista_numero)):
    if lista_numero[j] < 0:
        lista_numero[j] = 0

print(lista_numero)
~~~

## Questão 6

~~~py
lista_letras = ['d', 'i', 'a', ' ', 'd', 'e', ' ', 'a', 'u', 'l', 'a']

palavra = ''

for i in lista_letras:
    palavra += i

print(palavra)


print("====================================")

#Caminho inverso

lista_palavra = list()

frase = input("Digite uma frase qualquer: ")

for i in frase:
    lista_palavra.append(i)

print(lista_palavra)
~~~

## Desafio

~~~py
lista1 = [1,  2,  3,  4,  5,  6,  7,  8,  9]
lista2 = [10, 11, 12, 13, 14, 15, 16, 17, 18]
lista3 = [19, 20, 21, 22, 23, 24, 25, 26, 27]

lista_final = list()

lista_final += lista1[:3] + lista2[3:6] + lista3[6:]

print(lista_final)
~~~

## Atividades Python

<https://github.com/infinity-repositorios/atividades/blob/main/guias/Python.md>

## Menu

<https://github.com/infinity-repositorios/atividades>
