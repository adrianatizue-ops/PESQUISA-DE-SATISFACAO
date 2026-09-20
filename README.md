# Pesquisa de satisfação - Empresa TudoWeb

# Inicialização dos contadores
excelente = 0
bom = 0
ruim = 0

# Pesquisa com 50 entrevistados
for i in range(1, 51):
    print(f"\n--- Entrevistado {i} ---")

    nome = input("Digite o nome: ")
    idade = int(input("Digite a idade: "))

    print("\nOpinião sobre o atendimento:")
    print("1 - EXCELENTE")
    print("2 - BOM")
    print("3 - RUIM")

    opiniao = int(input("Digite sua opinião (1, 2 ou 3): "))

    # Verifica a opinião informada
    if opiniao == 1:
        excelente += 1
        print("Opinião registrada: EXCELENTE")

    elif opiniao == 2:
        bom += 1
        print("Opinião registrada: BOM")

    elif opiniao == 3:
        ruim += 1
        print("Opinião registrada: RUIM")

    else:
        print("Opinião inválida. Resposta não contabilizada.")

# Exibe o resultado da pesquisa
print("\n===== RESULTADO DA PESQUISA =====")
print(f"Total de entrevistados: 50")
print(f"Respostas EXCELENTE: {excelente}")
print(f"Respostas RUIM: {ruim}")
