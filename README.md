#Objetivo de criar uma calcula capaz de receber 2 numeros do usuario e fazer a soma deles (OK)
#Encontrar uma maneira para que o código seja repetido caso o usuário digite que quer realizar mais uma conta (OK)
#Tentar inplementar os calculos de subtração, multiplicação e divisão (OK)
#Criar uma interface gráfica para melhor experiencia do usuario ()

def add(x, y): #Função para realizar a soma
    return x + y

def sub(x, y): #Função para realizar a subtração
    return x - y

def mult(x, y): #Função para realizar a multiplicação
    return x * y

def div(x, y): #Função para realizar a divisão
    return x / y

def Radd(): #Função que realiza o calculo e retorna a resposta
    num1 = float(input("Digite o primeiro numero: "))
    num2 = float(input("\nDigite o segundo numero: "))
    print('\nO resultado da soma é ', num1, "+", num2, "=", add(num1, num2))

def Rsub():  # Função que realiza o calculo e retorna a resposta
    num1 = float(input("Digite o primeiro numero: "))
    num2 = float(input("\nDigite o segundo numero: "))
    print('\nO resultado da soma é ', num1, "-", num2, "=", sub(num1, num2))

def Rmult():  # Função que realiza o calculo e retorna a resposta
    num1 = float(input("Digite o primeiro numero: "))
    num2 = float(input("\nDigite o segundo numero: "))
    print('\nO resultado da soma é ', num1, "*", num2, "=", mult(num1, num2))

def Rdiv():  # Função que realiza o calculo e retorna a resposta
    num1 = float(input("Digite o primeiro numero: "))
    num2 = float(input("\nDigite o segundo numero: "))
    print('\nO resultado da soma é ', num1, "/", num2, "=", div(num1, num2))


def opcao(): # Mostra as opções e leva o usuário para a opção desejada
    while True:
        opcao = input('Escolha uma das opções abaixo:\n'
          '1- Adição\n'
          '2- Subtração\n'
          '3- Multiplicação\n'
          '4- Divisão\n'
          '0- Para Sair')
        if opcao == '1':
            return Radd()
        elif opcao == '2':
            return Rsub()
        elif opcao == '3':
            return Rmult()
        elif opcao == '4':
            return Rdiv()
        elif opcao == '0':
            print('\nObrigado, Até a próxima!')
            break
        else:
            print("Por favor, digite uma das opções.")


opcao() #Roda o menu
