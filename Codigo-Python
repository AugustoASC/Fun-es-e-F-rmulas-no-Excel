```python
# Recebe a entrada do usuário e armazena na variável "entrada"
entrada = input("Digite a descrição da função desejada: ")

def identificar_funcao_data(descricao):
    """
    Recebe uma descrição textual e retorna a fórmula Excel correspondente.
    Se a descrição não for reconhecida, retorna 'Função não encontrada'.
    """
    if descricao == "Retorna o dia do mês de uma data.":
        return "=DIA(A1)"

    elif descricao == "Retorna o mês de uma data.":
        return "=MÊS(A1)"

    elif descricao == "Retorna o ano de uma data.":
        return "=ANO(A1)"

    elif descricao == "Retorna a data e hora atuais.":
        return "=AGORA()"

    else:
        return "Função não encontrada"

# Exibe a fórmula correspondente à descrição fornecida
print(identificar_funcao_data(entrada))
