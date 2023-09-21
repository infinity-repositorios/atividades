# Atividades aula 4

## Funções

## Questão 1

~~~py
def tempo(seg):
    horas = seg // 3600
    seg -= horas * 3600

    min = seg // 60
    seg -= min * 60

    return f"{horas} : {min} : {seg}"

seg = int(input("Digite a quantidade de segundos que a fabrica está rodando: "))

print(tempo(seg))
~~~

## Questão 2

~~~py
def tempo_dias(anos, meses, dias):
    total_dias = int((anos * 365.25) + (meses * 30.4167) + dias)
    return total_dias

anos = int(input("Digite quanto anos você tem: "))
meses = int(input("Digite quanto meses você tem: "))
dias = int(input("Digite quanto dias você tem: "))

print(tempo_dias(anos, meses, dias))
~~~

## Questão 3

~~~py
def verificacao(inteiro):
    if inteiro >= 0:
        if inteiro % 2 == 0:
            return "Numero positivo e par"
        else:
            return "Numero positivo e impar"
    else:
        return "Numero negativo"
    
num = int(input("Digite um numero inteiro qualquer: "))

print(verificacao(num))
~~~

## Questão 4

~~~py
def volume_esfera(raio):
    volume = 4 / 3 * 3.14 * (raio ** 3)
    return volume

raio = float(input("Digite o raio de uma esfera, para calcular o volume: "))

print(volume_esfera(raio))
~~~

## Questão 5

~~~py
def fatorial(num):
    total = 1
    for i in range(1, num + 1):
        total *= i

    return total

num = int(input("Digite um numero inteiro e positivo: "))

print(fatorial(num))
~~~

## Questão 6

~~~py
def calculo(num):
    valor = 0
    texto = "S = "

    for i in range(1, num + 1):
        valor += 1 / i
        
        if i == 1:
            texto += f"1 "
        else:
            texto += f"+ 1/{i} "

    texto += f"= {valor:.2f}"

    return texto

num = int(input("Digite um valor inteiro e positivo: "))

print(calculo(num))
~~~

## Atividades Python

<https://github.com/infinity-repositorios/atividades/blob/main/guias/Python.md>

## Menu

<https://github.com/infinity-repositorios/atividades>
