# Previsão de Consumo de Dados de Rede

## Introdução
Este projeto tem como objetivo prever o consumo de dados móveis utilizando o Azure Machine Learning. A previsão precisa do consumo de dados é crucial para operadoras de telecomunicações, permitindo uma melhor gestão de recursos e otimização de serviços.

## Descrição dos Dados
Os dados utilizados neste projeto foram coletados de [fonte dos dados]. O conjunto de dados inclui variáveis como:
- Usuário ID
- Mês
- Quantidade de dados consumidos (MB)
- [Outras variáveis relevantes]

Exemplo de registro dos dados:
| Usuário ID | Mês | Dados Consumidos (MB) | ... |
|------------|-----|-----------------------|-----|
| 1          | Jan | 500                   | ... |

## Pré-processamento dos Dados
Os dados foram limpos e preparados da seguinte forma:
- Tratamento de valores ausentes
- Normalização dos dados
- Divisão em conjuntos de treinamento (80%) e teste (20%)

## Escolha do Modelo
Optamos por utilizar a Regressão Linear devido à sua simplicidade e eficácia em problemas de previsão contínua. Outras alternativas consideradas foram [algoritmos] mas foram descartadas por [razões].

## Treinamento do Modelo
O modelo foi treinado com os seguintes hiperparâmetros:
- [Hiperparâmetro 1]: valor
- [Hiperparâmetro 2]: valor

Gráfico de evolução do treinamento:
!Gráfico de Treinamento

## Avaliação do Modelo
Utilizamos as seguintes métricas para avaliar o modelo:
- Erro Quadrático Médio (MSE): valor
- [Outras métricas]

Gráfico de comparação entre valores previstos e reais:
!Gráfico de Comparação

## Publicação do Modelo
O modelo foi publicado como um serviço web no Azure Machine Learning. As configurações dos pontos de extremidade são as seguintes:
- URL do Endpoint: [URL]
- Chave de API: [Chave]

## Exemplos de Uso
### Python
```python
import requests

url = "https://seu-endereco-de-endpoint"
api_key = "sua-chave-de-api"
data = {"input": [valores]}

response = requests.post(url, headers={"Authorization": f"Bearer {api_key}"}, json=data)
print(response.json())
