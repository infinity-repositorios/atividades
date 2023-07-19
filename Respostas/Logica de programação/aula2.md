# Condicionais:
## Questão 1:
~~~py
num = float(input('Digite um numero qualquer Real: '))

if num > 0:
    if num % 2 == 0:
        print(f'O numero {num} é par')
    else:
        print(f'O numero {num} é impar')
elif num < 0:
    print(num ** 2)
else:
    print('Numero igual a zero')
~~~
## Questão 2:
~~~py
temp = float(input('Digite o valor da tempera da pessoa: '))

if temp <= 37:
    passagem = True
else:
    passagem = False

print(f'Após a verificação de acordo com o resultado sendo ele:\n'
      f'True para passagem liberada e \n'
      f'False para barrrado:\n'
      f'{passagem}')
~~~
## Questão 3:
~~~py
indice = float(input('Digite o valor do indice de poluição: '))
if 0.05 <= indice < 0.25:  # indice >= 0.05 and indice < 0.25
    print('Aceitavél')
elif indice <= 0.04:
    print('1° grupo, atividades suspensas')
elif indice <= 0.05:
    print('1° e 2° grupo, atividades suspensas')
elif indice > 0.05:
    print('Todos os grupo, atividades suspensas')

~~~
## Questão 4:
~~~py
timeA = input('Digite o nome do primeiro time: ')
timeB = input('Digite o nome do segundo time: ')

golsA = int(input(f'Digite os gols do time {timeA}: '))
golsB = int(input(f'Digite os gols do time {timeB}: '))

if golsA > golsB:
    print(f'O time {timeA} venceu o time {timeB}')
elif golsA < golsB:
    print(f'O time {timeB} venceu o time {timeA}')
else:
    print('Os times empataram')
~~~
## Questão 5:
~~~py
precoA = float(input('Digite o valor 1: '))
precoB = float(input('Digite o valor 2: '))
precoC = float(input('Digite o valor 3: '))

if precoA < precoB and precoA < precoC:
    print(f'O valor de {precoA}R$ deve ser comprado')
elif precoB < precoC and precoB < precoA:
    print(f'O valor de {precoB}R$ deve ser comprado')
else:
    print(f'O valor de {precoC}R$ deve ser comprado')
~~~
## Questão 6:
~~~py
num_empre = int(input("Digite o codigo do empregado: "))
ano_nasci = int(input("Digite o ano de nascimento do empregado: "))
ano_ingre = int(input("Digite o ano de ingresso do empregado: "))

idade = 2022 - ano_nasci
tp_tra = 2022 - ano_ingre

if idade >= 65 or tp_tra >= 30 or (idade >= 60 and tp_tra >= 25):
    print(f"O empregado de codigo: {num_empre} com {idade} anos e {tp_tra} de empresa pode requerer aposentadoria")
else:
    print("Não pode requerer a aposentadoria")
~~~

## Atividades lógica: <br>
https://github.com/infinity-repositorios/atividades/blob/main/guias/Lógica%20da%20Programação.md
## Menu:
https://github.com/infinity-repositorios/atividades