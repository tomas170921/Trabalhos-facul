def converter_moeda(valor, de_moeda, para_moeda):
    # Taxas de câmbio fixas (exemplo)
    taxas = {
        'USD': 1.0,  # Dólar americano
        'EUR': 0.85,  # Euro
        'BRL': 5.25,  # Real brasileiro
        'JPY': 110.0,  # Iene japonês
    }

    if de_moeda not in taxas or para_moeda not in taxas:
        print("Uma das moedas não é válida.")
        return None

    # Converter valor para USD primeiro
    valor_em_usd = valor / taxas[de_moeda]

    # Converter de USD para a moeda de destino
    valor_convertido = valor_em_usd * taxas[para_moeda]
    return valor_convertido


def main():
    valor = float(input("Digite o valor que deseja converter: "))
    de_moeda = input("Digite a moeda de origem (USD, EUR, BRL, JPY): ").upper()
    para_moeda = input("Digite a moeda de destino (USD, EUR, BRL, JPY): ").upper()

    resultado = converter_moeda(valor, de_moeda, para_moeda)

    if resultado is not None:
        print(f"{valor} {de_moeda} é igual a {resultado:.2f} {para_moeda}")


if __name__ == "__main__":
    main()
