# Atividades aula 3

## Dicionarios e Sets

## Questão 1

~~~py
pessoas = [
    {"nome": "João", "idade": 30},
    {"nome": "Maria", "idade": 25},
    {"nome": "Pedro", "idade": 35},
    {"nome": "Ana", "idade": 28},
    {"nome": "Carlos", "idade": 40}
]

nome = input("Digite um nome para se buscar na lista de pessoas cadastradas: ")

contagem = 0

for i in pessoas:
    if nome == i["nome"]:
        print(f"A pessoa {nome}, tem {i['idade']}")
        break
    
    contagem += 1

if contagem == 5:
    print("Pessoa não encontrada")
~~~

## Questão 2

~~~py
agenda = dict()

while True:
    escolha = int(input("Digite uma das opções:\n" +
                        "1 - Adicionar Contato;\n" +
                        "2 - Ver todos os contatos;\n" +
                        "0 - Finalizar Sistema;\n"))
    
    match escolha:
        case 1:
            nome = input("Digite o nome do contato: ")
            numero = int(input("Digite o numero do contato: "))

            agenda[numero] = nome

        case 2:
            for numero, nome in agenda.items():
                print(f"{nome} -> {numero}")
            
        case 0:
            break

        case _:
            print("Opção Invalida")  
~~~

## Questão 3

~~~py
alunos = dict()

matricula = 1

while True:
    escolha = int(input("Digite uma das opções:\n" +
                        "1 - Adicionar novo aluno: \n" +
                        "2 - Ver todos os alunos: \n" +
                        "3 - Finaliar sistema: \n"))
    
    match escolha:
        case 1:
            nome = input("Digite o nome do aluno: ")
            idade = int(input("Digite a idade do aluno: "))
            sexo = input("Digite o sexo do aluno: ")

            alunos[matricula] = [nome, idade, sexo]

            matricula += 1

        case 2:
            for matricula, info in alunos.items():
                print(f"O aluno de matricula: {matricula} tem as seguintes informações:\n" +
                      f"nome - {info[0]} | idade - {info[1]} | sexo - {info[2]}")

        case 0:
            break

        case _:
            print("Opção invalida")        
~~~

## Desafio

~~~py
pacientes = dict()
id = 1

while True:
    escolha = int(input("Digite uma das opções:\n" +
                        "1 - Cadastrar novo paciente;\n" +
                        "2 - Ver todos os pacientes;\n" +
                        "3 - Apagar paciente;\n" +
                        "0 - Finalizar sistemas.\n"))
    
    match escolha:
        case 1:
            nome = input("Digite o nome do paciente: ")
            idade = int(input("Digite a idade do paciente: "))
            peso = float(input("Digite o peso do paciente: "))
            altura = float(input("Digite o altura do paciente: "))

            pacientes[id] = [nome, idade, peso, altura]

            id += 1

        case 2:
            for x, paciente in pacientes.items():
                print(f"Paciente de id {x} -> {paciente}") 
        
        
        case 3:
            escolha = int(input("Procurar paciente por:\n" +
                                "1 - ID;\n" +
                                "2 - Nome.\n"))

            match escolha:
                case 1:
                    deletado = int(input("Digite o id do paciente: "))

                    pacientes.pop(deletado)
                
                case 2:
                    deletado = input("Digite o nome do paciente: ")
                    contagem = 1

                    for i in pacientes:
                        if deletado == pacientes[i][0]:
                            pacientes.pop(i)
                            break
                case _:
                    print("Opção inexistente")

        case _:
                    print("Opção inexistente")   
~~~

## Atividades Python

<https://github.com/infinity-repositorios/atividades/blob/main/guias/Python.md>

## Menu

<https://github.com/infinity-repositorios/atividades>
