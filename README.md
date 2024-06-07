# Projeto: Simulação e Análise de Velocidades de Correntes Marinhas

### Código em Python para Monitoramento de Correntes Marinhas com Gráficos

Este código simula a coleta e análise de dados de velocidade e temperatura das correntes marinhas, atendendo aos requisitos especificados. Ele inclui variáveis, tipos de dados, estruturas de controle, manipulação de listas e strings, funções, estruturas de dados, manipulação de arquivos e tratamento de exceções. Além disso, gera gráficos para visualização dos dados.

## Grupo BlueVison
- Gilson Dias ............................... RM552345 
- Gustavo Bezerra ..................... RM553076 

#### Descrição do Código

1. **Coleta de Dados**: Simula a coleta de dados de velocidade e temperatura das correntes marinhas em diferentes pontos.
2. **Análise de Dados**: Determina se os dados estão em estado "normal" ou "crítico" com base em critérios definidos.
3. **Armazenamento de Dados**: Salva os resultados em um arquivo JSON.
4. **Leitura de Dados**: Lê os dados do arquivo JSON e exibe no console.
5. **Visualização de Dados**: Gera gráficos para visualização das velocidades e temperaturas das correntes marinhas.

### Explicação do Código

1. **Coleta de Dados**:
   - `coletar_dadosVelocidade`: Gera uma lista de velocidades aleatórias entre 0 e 16 m/s.
   - `coletar_dadosTemperatura`: Gera uma lista de temperaturas aleatórias entre -5 e 40 °C.

2. **Análise de Dados**:
   - `analisar_dados`: Determina se os dados estão em estado "normal" ou "crítico" com base em critérios definidos. Adiciona uma coluna "Status" ao DataFrame.

3. **Armazenamento de Dados**:
   - `salvar_dados`: Salva os dados coletados e os resultados da análise em um arquivo JSON. Utiliza tratamento de exceções para lidar com possíveis erros de escrita.

4. **Leitura de Dados**:
   - `ler_dados`: Lê o conteúdo do arquivo JSON e retorna os dados. Utiliza tratamento de exceções para lidar com possíveis erros de leitura.

5. **Visualização de Dados**:
   - `criar_graficos`: Gera gráficos de dispersão para visualizar as velocidades e temperaturas das correntes marinhas. Utiliza cores diferentes para indicar o status "normal" ou "crítico".

6. **Função Principal**:
   - `main`: Coordena a coleta, análise, armazenamento e visualização dos dados. Define o número de pontos de coleta, chama as funções apropriadas e exibe os resultados.


## Requisitos

- Python 3.7 ou superior

## Dependências

As seguintes bibliotecas Python são necessárias:

- `random` (biblioteca padrão do Python)
- `json` (biblioteca padrão do Python)
- `pandas` (`pip install pandas`)
- `matplotlib` (`pip install matplotlib`)

4. **Resultado Esperado:**
   - O script irá gerar um conjunto de dados simulados de velocidades e temperatura das correntes marinhas.
   - Verifica se as correntes marinhas estao e em estado 'normal' ou 'critico'
   - Salvará esses dados e estatísticas em um arquivo `dados_correntes.json`.
   - Lerá o arquivo JSON e exibirá os dados no console.
   - Criará gráficos que serão exibidos no final do código.


### Conclusão

Este código atende aos requisitos especificados, utilizando conhecimentos básicos em Python, manipulação de listas e strings, funções, estruturas de dados, manipulação de arquivos e tratamento de exceções. Ele simula a coleta e análise de dados de correntes marinhas, salvando e lendo os resultados de um arquivo JSON, e gera gráficos para visualização dos dados.