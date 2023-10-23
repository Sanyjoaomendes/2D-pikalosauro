# 2D-pikalosauroimport random

def adivinhacao():
    numero_secreto = random.randint(1, 100)
    tentativas = 0

    print("Bem-vindo ao jogo de adivinhação!")
    print("Eu escolhi um número entre 1 e 100. Tente adivinhar!")

    while True:
        palpite = int(input("Seu palpite: "))

        tentativas += 1

        if palpite == numero_secreto:
            print(f"Parabéns! Você acertou em {tentativas} tentativas.")
            break
        elif palpite < numero_secreto:
            print("Tente um número maior.")
        else:
            print("Tente um número menor.")

if __name__ == "__main__":
    adivinhacao()
