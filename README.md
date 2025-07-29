# Calculadora
Repositório que mostra e demonstra uma atividade que tinha como objetivo de criar uma calculadora

calculadora:
import math
import os

def soma(a,b):
    x = a + b  # soma
    return x

def subtração(a,b):
    x = a - b   # subtração
    return x

def divisão(a,b):
    if a == 0 or b == 0:
        print("Não é possivel ser divisivel por 0")
    x = a / b # divisão
    return x

def multiplicação(a,b):
    x = a * b   # multiplicação
    return x


def potenciação(a,b):
    return math.pow(a,b) # portenciação

def raizquadrada(x):
    if x < 0:        
        print("Erro, número inválido!")
    # raiz quadrada
    return math.sqrt(x)

def fatorial(x):
    if x < 0 and not int: #  fatorial
        print("Erro, número inválido!")
    return math.factorial(int(x))

def seno(x): 
    return math.sin(math.radians(x))

def coseno(x):
    return math.cos(math.radians(x)) # razões trigonométricas

def tangente(x):
    return math.tan(math.radians(x))

def logaritmo_base_10(x):
    if x < 0:
        print("Erro, número inválido!") # logaritmo de base 10
    print(math.log10(x))
    return x

def logaritmo_base_e(x):
    if x < 0:
        print("Erro, número inválido!") # logaritmo de base e
    print(math.log(x))
    return x

def menu():
    print("Bem vindo a calculadora científica, faça a sua escolha")
    print("1 = soma")
    print("2 = subtrair")
    print("3 = divisão")
    print("4 = multiplicação")
    print("5 = potenciação")   # menu da calculadore científica
    print("6 = raiz quadrada")
    print("7 = fatorial")
    print("8 = razões trigonométricas")
    print("9 = logaritmo")
    print("0 = sair")

menu()

escolha = -1

while escolha != 0:
    menu()
    escolha = int(input("Digite sua escolha\n-->"))
    if escolha == 1:
        os.system("cls")
        print("\tsoma\n")
        a = float(input("Digite o primeiro valor\n-->"))
        b = float(input("Digite o segundo valor\n-->"))
        os.system("pause") # soma
        os.system("cls")
        print(soma(a,b))
        os.system("pause")


    elif escolha == 2:
        os.system("cls")
        print("\tsubtração\n")
        a = float(input("Digite o primeiro valor\n-->"))
        b = float(input("Digite o segundo valor\n-->"))
        os.system("pause") # subtração
        os.system("cls")
        print(subtração(a,b))
        os.system("pause")


    elif escolha == 3:
        os.system("cls")
        print("\tdivisão\n")
        a = float(input("Digite o primeiro valor\n-->"))
        b = float(input("Digite o segundo valor\n-->"))
        os.system("pause") # divisão
        os.system("cls")
        print(divisão(a,b))
        os.system("pause")

    elif escolha == 4:
        os.system("cls")
        print("\tmultiplicação\n")
        a = float(input("Digite o primeiro valor\n-->"))
        b = float(input("Digite o segundo valor\n-->"))
        os.system("pause") # multiplicação
        os.system("cls")
        print(multiplicação(a,b))
        os.system("pause")

    elif escolha == 5:
        os.system("cls")
        print("\tpotenciação\n")
        a = int(input("Digite o primeiro valor\n-->"))
        b = int(input("Digite o segundo valor\n-->"))
        os.system("pause") # potenciação
        os.system("cls")
        print(potenciação(a,b))
        os.system("pause")


    elif escolha == 6:
        os.system("cls")
        print("\traiz quadrada\n")
        x = int(input("Digite um número\n-->"))
        os.system("pause") # raiz quadrada
        os.system("cls")
        print(raizquadrada(x))
        os.system("pause")


    elif escolha == 7:
        os.system("cls")
        print("\tfatorial\n")
        x = int(input("Digite o número\n-->"))
        os.system("pause") # fatorial
        os.system("cls")
        print(fatorial(x))
        os.system("pause")


    elif escolha == 8:
        os.system("cls")
        print("\tseno - 1\ncoseno - 2\ntangente - 3")
        razõestrigonométricas = int(input("Escolha uma das razões trigonométricas\n-->"))
        os.system("pause")            # razões trigonométricas
        os.system("cls") 
        if razõestrigonométricas == 1:
            print("\tseno\n")            # seno
            x = int(input("Digite um número\n-->"))
            os.system("pause")
            os.system("cls")
            print(seno(x))
            os.system("pause")


        elif razõestrigonométricas == 2 :
            os.system("cls")
            print("\tcoseno\n")
            x = int(input("Digite um número\n-->"))
            os.system("pause")           #coseno
            os.system("cls")
            print(coseno(x))
            os.system("pause")


        elif razõestrigonométricas == 3:
            os.system("cls")
            print("\ttangente\n")
            x = int(input("Digite um número\n-->"))
            os.system("pause")
            os.system("cls")            #tangente
            print(tangente(x))
            os.system("pause")

        else:
            os.system("cls")
            print("Erro, número inválido")
            os.system("pause")
    
    elif escolha == 9:
        os.system("cls")
        print("logaritmo de base 10 = 1\nlogaritmo de base e = 2")
        logaritmo = int(input("Escolha o opção logaritmica\n-->"))
        os.system("pause")
        if logaritmo == 1:
            os.system("cls")
            print("\tlogaritmo de base 10\n") # lagaritmo
            x = int(input("Digite um número\n-->"))
            os.system("pause")
            os.system("cls")
            print(logaritmo_base_10(x))
            os.system("pause")


        elif logaritmo == 2:
            os.system("cls")
            print("\tlogaritmo de base e\n")
            x = int(input("Digite um número\n-->"))
            os.system("pause")
            os.system("cls")
            print(logaritmo_base_e(x))
            os.system("pause")

        else:
            print("Número inválido!")
        
    elif escolha < 0:
        os.system("cls")
        print("Número negativo não encontrado!")
        os.system("pause")
    
    elif escolha > 9:
        os.system("cls")
        print("Número inválido!")
        os.system("pause")

print("Saindo...")
  
todo:
import os

escolha = 4

qtd = int(input("Digite a quantidade de tarefas que deseja colocar\n-->"))
tarefa = [input(f"\nDigite a sua {i+1}° tarefa\n-->") for i in range(qtd)]

os.system("cls")
while escolha != 0:
    print("1 = Completar tarefa\n2 = adicionar\n3 = excluir\n4 = editar\n0 = *sair*\t")   # Opções/Ações na lista
    
    for t in tarefa:
        print(f" - {t}\t")
    
    
    escolha = int(input("Digite qual é sua escolha\n-->"))

    if escolha == 1:
        completa = int(input("Qual tarefa você completou?\n-->"))
        if completa >= 0 and completa <= qtd:
            tarefa[completa] += "- OK"                               # Tarefas completas
            for t in tarefa:
                print(t)
        else:
            print("Tarefa inválida")
    

    elif escolha == 2:
        tarefa.append(input("Digite a sua tarefa adicional\n-->")) 
        qtd += 1                                                      # Adoção de tarefas
        for t in tarefa:
            print(t)

    elif escolha == 3:
        for t in tarefa:
            print(t)
        excluir = int(input(f"Qual tarefa voce deseja excluir\n-->"))
        if excluir >= 0 and excluir <= qtd:                           # Exclusão de tarefas
            excluir -= 1
            tarefa.pop(excluir)
            
    
    elif escolha == 4:
        editar = int(input("Digite qual tarefa queira editar\n-->"))
        if editar >= 0 and editar <= qtd:
            tarefa[editar] = str(input("Digite sua edição\n-->"))
            for t in tarefa:
                print(t)

    else:
        ("Digite um número válido")
os.system("pause")

print("Saindo...")



    





