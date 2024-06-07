# Projeto: Simulação e Análise de Velocidades de Correntes Marinhas

Este projeto realiza a simulação de coleta de dados de velocidades de correntes marinhas, analisa esses dados, salva os resultados em um arquivo JSON e cria gráficos para visualização.

## Grupo BlueVison
- Gilson Dias ............................... RM552345 
- Gustavo Bezerra ..................... RM553076 

## Descrição do Projeto

O projeto é composto por um script Python que:
1. Gera dados simulados de velocidades de correntes marinhas e temperatura.
2. Verifica se velocidade e a temperatura das correntes marinhas normais ou em estado critico.
3. Salva os dados e as estatísticas em um arquivo JSON.
4. Lê os dados do arquivo JSON e exibe-os em 2 graficos, um de velociade e outro de temperatura.

## Estrutura do Projeto

- `coletar_dados(num_pontos)`: Função que gera uma lista de velocidades aleatórias.
- `analisar_dados(dados)`: Função que calcula a média, máxima e mínima das velocidades.
- `salvar_dados(nome_arquivo, dados, media, maxima, minima)`: Função que salva os dados em um arquivo JSON.
- `ler_dados(nome_arquivo)`: Função que lê os dados de um arquivo JSON e os exibe no console.
- `criar_graficos(dados)`: Função que cria gráficos das velocidades e das estatísticas.
- `main()`: Função principal que coordena a execução de todas as outras funções.

## Requisitos

- Python 3.7 ou superior

## Dependências

As seguintes bibliotecas Python são necessárias:

- `random` (biblioteca padrão do Python)
- `json` (biblioteca padrão do Python)
- `pandas` (`pip install pandas`)
- `matplotlib` (`pip install matplotlib`)

## Instruções de Uso

1. **Clone o repositório ou copie o código para um diretório local.**

2. **Instale as dependências:**
   ```bash
   pip install pandas matplotlib
   ```

3. **Execute o script:**
   ```bash
   python gs_python.ipynb
   ```
   Onde `gs_python.ipynb` é o nome do arquivo onde o código está salvo.

4. **Resultado Esperado:**
   - O script irá gerar um conjunto de dados simulados de velocidades de correntes marinhas.
   - Calculará a média, máxima e mínima dessas velocidades.
   - Salvará esses dados e estatísticas em um arquivo `dados_correntes.json`.
   - Lerá o arquivo JSON e exibirá os dados no console.
   - Criará gráficos que serão exibidos no final do código.

## Arquivo JSON de Saída

O arquivo `dados_correntes.json` terá o seguinte formato:
```json
{
    "velocidades": [1.23, 2.34, 1.78, ...],
    "media": 1.85,
    "maxima": 2.90,
    "minima": 0.75
}
```

## Exemplo de Execução

```python
if __name__ == "__main__":
    main()
```

Ao executar o script, você verá a coleta de dados simulada, os resultados das estatísticas exibidos no console e gráficos exibidos em uma janela de visualização.

