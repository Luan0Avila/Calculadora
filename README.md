#Objetivo de criar uma calcula capaz de receber 2 numeros do usuario e fazer a soma deles
#Encontrar uma maneira para que o código seja repetido caso o usuário digite que quer realizar mais uma conta (OK)
#Tentar inplementar os calculos de subtração, multiplicação e divisão ( )
#Criar uma interface gráfica para melhor experiencia do usuario ()
def add(x, y): #Função para realizar a soma
    return x + y
def conta(): #Função que realiza o calculo e retorna a resposta
    num1 = float(input("Digite o primeiro numero: "))
    num2 = float(input("\nDigite o segundo numero: "))
    print('\nO resultado da soma é ', num1, "+", num2, "=", add(num1, num2))


print("Olá, bem-vindo!\nEsta é a calculadora de soma\n")
def menu(): #Função do menu
    while True: #Cria uma repetição para a conta
        pergunta = input("Deseja realizar uma conta? (sim/não) ")
        if pergunta.lower() == "não": #fecha o programa caso a resposta seja 'não'
            print("Obrigado até mais!")
            break
        elif pergunta.lower() == "sim":
            conta()
        else: #rejeita respostas que não sejam de sim ou não
            print("Por favor, digite 'sim' ou 'não'.")
menu()


