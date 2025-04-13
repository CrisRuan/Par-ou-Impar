import random

while True:

    valor1 = int(input("Digite um valor:  "))
    pi = str(input("Par[P] ou Impar[I]:  ")).upper()

    comp = random.randint(0, 10)
    soma = comp + valor1

    print(f"Você escolheu {valor1}, eu escolhi {comp}.")
    print(f"A soma é igual a {valor1 + comp}.")

    if (soma % 2 == 0):
        print("O resultado deu Par!")
        if pi == "P":
            print("Você Ganhou!")
        else:
            print("Você Perdeu!")
    else:
        print("O resultado deu Ímpar!")
        if pi == "I":
            print("Você Ganhou!")
        else:
            print("Você Perdeu")

    continuar = str(input("Deseja jogar novamente? [S/N]")).upper()
    if (continuar == "N"):
        break

print("========================")
print("=== FIM DO PROGRAMA! ===")
print("==== Até a Próxima) ====")
print("========================")
