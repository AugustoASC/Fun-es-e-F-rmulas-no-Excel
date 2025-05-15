# 📅 Funções de Data e Hora no Excel - Identificador de Fórmulas

---

## 📝 Descrição

Este projeto é um **programa em Python** que recebe uma descrição textual de uma função de manipulação de data e hora no Excel e retorna a fórmula exata correspondente.

O Excel possui diversas funções para trabalhar com datas e horas, permitindo calcular intervalos, extrair partes específicas de uma data e obter valores temporais formatados. Essas funções são essenciais para análise e manipulação de dados temporais em planilhas.

Aqui, você insere uma breve descrição da operação desejada, e o programa devolve a fórmula correta do Excel para essa ação.

---

## 🔍 Funções Excel Reconhecidas

| Descrição                                      | Fórmula Excel  |
| ---------------------------------------------- | -------------- |
| Retorna o dia do mês de uma data.              | `=DIA(A1)`     |
| Retorna o mês de uma data.                      | `=MÊS(A1)`     |
| Retorna o ano de uma data.                      | `=ANO(A1)`     |
| Retorna a data e hora atuais do sistema.       | `=AGORA()`     |

---

## 🚀 Como o programa funciona

- O usuário insere uma **descrição textual** da função desejada.
- O programa verifica essa descrição e **retorna a fórmula correspondente** do Excel.
- Caso a descrição não seja reconhecida, retorna a mensagem:  
  **"Função não encontrada"**.

---

## 💻 Código-fonte

```python
# Recebe a entrada do usuário e armazena na variável "entrada"
entrada = input()

# Função responsável por receber uma descrição e retornar a fórmula correspondente do Excel.
def identificar_funcao_data(descricao):
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

# Imprime a fórmula correspondente à entrada fornecida
print(identificar_funcao_data(entrada))

