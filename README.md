# calculadora-imc
Calculadora simples para calcular o Índice de Massa Corporal (IMC) e classificar o resultado em faixas de peso. # Linguagem  - Python## Como usar  - Execute o programa - Informe seu peso em kg e sua altura em metros - Veja o resultado do IMC e a classificação 

def calcular_imc():
    peso = float(input("Qual o seu peso (kg)? "))
    altura = float(input("Qual a sua altura (m)? "))

    imc = peso / (altura ** 2)
    print(f"Seu IMC é: {imc:.1f}")

    if imc < 18.5:
        print("Você está Abaixo do Peso.")
    elif 18.5 <= imc <= 24.9:
        print("Você está no Peso Ideal.")
    elif 25 <= imc <= 29.9:
        print("Você está com Pré-Obesidade.")
    elif 30 <= imc <= 34.9:
        print("Você está com Obesidade Moderada.")
    elif 35 <= imc <= 39.9:
        print("Você está com Obesidade Severa.")
    else:
        print("Você está com Obesidade Mórbida.")

calcular_imc()
