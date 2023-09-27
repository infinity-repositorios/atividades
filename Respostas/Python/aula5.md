# Atividades aula 5

## Funções II

## Questão 1

~~~py
numero = float(input('Digite um numero qualquer positivo e real: '))

ver = lambda x: "Par" if x % 2 == 0 else "Impar"

print(ver(numero))
~~~

## Questão 2

~~~py
palavra1 = input("Digite a primeira palavra: ")
palavra2 = input("Digite a segunda palavra: ")

juncao = (lambda str1, str2: 
          str1 + str2 
          if len(str1) > 5 and len(str2) > 5 
          else 
          "Erro: as strings devem ter mais de 5 caracteres.")

print(juncao(palavra1, palavra2))
~~~

## Questão 3

~~~py
num = int(input("Digite um numero interiro qualquer: "))

ver = lambda x: "Divisivel" if x % 3 == 0 and x % 5 == 0 else "Não divisivel"

print(ver(num))
~~~

## Questão 4

~~~py
palavras = ['abacaxi', 'carro', 'computador', 'elefante', 'guitarra', 'janela', 'piscina', 'sapato', 'travesseiro', 'viagem']

maiscula = list(map(lambda x: x.upper(), palavras))

print(maiscula)
~~~

## Questão 5

~~~py
palavras = ['abacaxi', 'carro', 'computador', 'elefante', 'guitarra', 'janela', 'piscina', 'sapato', 'travesseiro', 'viagem']

nPalavras = list(filter(lambda x: len(x) > 5, palavras))

print(nPalavras)
~~~

## Questão 6

~~~py
from functools import reduce

numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

soma = reduce(lambda x, y: x + y, numeros)

print(soma)
~~~

## Questão 7

~~~py
pessoas = [
    {'nome': 'João', 'idade': 31},
    {'nome': 'Maria', 'idade': 37},
    {'nome': 'José', 'idade': 39},
    {'nome': 'Ana', 'idade': 28},
]

nomes = list(map(lambda p: p['nome'], pessoas))

print(nomes)
~~~

## Atividades Python

<https://github.com/infinity-repositorios/atividades/blob/main/guias/Python.md>

## Menu

<https://github.com/infinity-repositorios/atividades>
