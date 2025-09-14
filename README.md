
## Contato
- Autor: Marcus Ferreira  
- [LinkedIn](https://www.linkedin.com/in/mvsilfer)  
- [GitHub](https://github.com/MVSilfer-Fer)

# Filtro Lag de Primeira Ordem

Este projeto é um **protótipo em Python** para aplicar e avaliar um filtro lag de primeira ordem (filtro exponencial) em sinais de processo industrial.  
Foi desenvolvido em formato de notebook para permitir exploração rápida e visual dos resultados.

## Funcionalidades
- Leitura de dados de processo a partir de **CSV ou Excel**.
- Aplicação de filtro digital de 1ª ordem parametrizado pela constante de tempo (τ).
- Geração de gráficos comparando **sinal original vs filtrado**.
- Estatísticas descritivas (média, mediana, desvio padrão, variância, correlação).
- Espectro de potências no domínio de períodos, evidenciando a atenuação de ruídos de alta frequência.

## Estrutura
- `notebook.ipynb` → código principal com filtro, gráficos e análise estatística.
- Dados de entrada → planilhas/arquivos CSV com séries temporais (exemplo em `data/`).

## Exemplo de Uso
1. Ajuste os parâmetros no notebook:
   ```python
   path = "data/Dados do processo para filtrar.xlsx"
   sheet = "FIC02"
   col_time = "Timestamp"
   col_var = "FIC02"
   tau = 120.0
   Ts = 1.0
   
   Execute as células para carregar os dados, aplicar o filtro e visualizar os resultados.

   Requisitos:

   Python 3.10+

   Bibliotecas:
   pandas
   numpy
   plotly
   openpyxl (para leitura de Excel)

   Instale tudo com:
   pip install -r requirements.txt