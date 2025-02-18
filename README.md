# Previsão de Consumo de Dados de Rede

Este repositório contém um modelo de previsão criado utilizando o Azure Machine Learning para prever o consumo de dados móveis.

### Passos para Criar o Modelo

1. **Configuração do Ambiente no Azure Machine Learning**:
   - Crie uma conta no Azure.
   - Acesse o portal do Azure e crie um workspace no Azure Machine Learning.

2. **Coleta e Preparação dos Dados**:
   - Utilize dados históricos de consumo de dados móveis. Esses dados podem incluir informações como a quantidade de dados consumidos por usuário, por mês, e outras variáveis relevantes.
   - Exemplos de fontes de dados podem ser relatórios de operadoras de telecomunicações ou datasets públicos.
  
  3. **Criação do Modelo de Previsão**:
   - No Azure Machine Learning, crie um novo experimento.
   - Carregue o conjunto de dados preparado.
   - Escolha um algoritmo de regressão, como a Regressão Linear, para prever o consumo de dados.
   - Treine o modelo com os dados históricos.

4. **Avaliação e Ajuste do Modelo**:
   - Avalie o desempenho do modelo utilizando métricas como o erro quadrático médio (MSE).
   - Ajuste os hiperparâmetros do modelo para melhorar a precisão.

5. **Configuração dos Pontos de Extremidade**:
   - Após treinar o modelo, publique-o como um serviço web.
   - Configure os pontos de extremidade (endpoints) para permitir o acesso ao modelo.
   - Anote a URL do endpoint e a chave de API gerada.
