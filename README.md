# Análise e Previsão de Casos de COVID-19 em MS com LSTM

![Python](https://img.shields.io/badge/Python-3.11-blue.svg)
![Libraries](https://img.shields.io/badge/Libraries-Pandas%20%7C%20TensorFlow%20%7C%20Matplotlib-orange.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

Este repositório contém o código e os dados do projeto de extensão desenvolvido para a disciplina de Projeto Integrador III do Curso Superior de Tecnologia de Ciência dos Dados da UFMS.

## 📜 Descrição do Projeto

O projeto visa analisar a evolução da pandemia de COVID-19 no estado de Mato Grosso do Sul, transformando dados públicos complexos em informações acessíveis e preditivas. Foram desenvolvidas duas soluções principais: uma **ferramenta de visualização interativa** e um **modelo de previsão de série temporal** utilizando uma rede neural recorrente (LSTM).

O objetivo é fornecer à comunidade uma forma clara e intuitiva de entender a relação entre casos, óbitos e vacinação, além de oferecer uma previsão de tendências futuras de casos confirmados.

## ✨ Principais Funcionalidades

* **Análise Exploratória de Dados (EDA):** Limpeza, tratamento e junção de múltiplas fontes de dados sobre a pandemia.
* **Dashboard Interativo:** Um gráfico interativo desenvolvido com Matplotlib e Ipywidgets que permite a exploração anual dos dados, com anotações de totais mensais para cada métrica (casos, óbitos e vacinas).
* **Modelo Preditivo:** Implementação de uma rede neural LSTM para prever a tendência de novos casos, treinada com técnicas como *Early Stopping* para otimizar a performance.
* **Avaliação de Performance:** O modelo foi avaliado com a métrica RMSE (Raiz do Erro Quadrático Médio) para quantificar sua precisão.

## 📊 Visualizações

### Dashboard Interativo de Análise Anual
Este gráfico permite a visualização consolidada dos dados, com um menu para selecionar o ano desejado.

*(**Instrução:** Tire um print do seu gráfico interativo, salve na pasta `images/` e substitua o link abaixo)*
`![Dashboard Interativo](images/grafico_interativo.png)`

### Performance do Modelo LSTM
Este gráfico compara os valores reais de casos confirmados com as previsões geradas pelo modelo no conjunto de teste.

*(**Instrução:** Salve a imagem do gráfico do modelo, salve na pasta `images/` e substitua o link abaixo)*
`![Performance do Modelo LSTM](images/resultado_lstm.png)`

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python 3
* **Bibliotecas Principais:**
    * **Análise de Dados:** Pandas, NumPy
    * **Machine Learning:** TensorFlow (Keras), Scikit-learn
    * **Visualização de Dados:** Matplotlib
    * **Interatividade:** Ipywidgets
* **Ambiente de Desenvolvimento:** Google Colab / Jupyter Notebook
* **Fontes de Dados:**
    * Painel de Monitoramento de Casos de COVID-19 - SES/MS
    * Vacinômetro COVID-19 - Ministério da Saúde


## 📈 Resultados do Modelo

O modelo LSTM treinado alcançou uma performance promissora para a previsão de casos diários.

* **RMSE (Raiz do Erro Quadrático Médio):** **18.74**
    * *Interpretação: Em média, as previsões do modelo desviam em aproximadamente 19 casos do valor real, um resultado considerado muito bom para a complexidade da série temporal.*

## 🚀 Melhorias Futuras

* Otimização dos hiperparâmetros do modelo LSTM (ex: número de neurônios, `batch_size`, etc.).
* Inclusão de novas *features* no modelo, como dados de mobilidade ou feriados.
* Desenvolvimento de um deploy da solução como uma aplicação web simples usando Streamlit ou Flask.

## ✍️ Autora

* **Denise Jeannie Marti**
    * LinkedIn: `[LINK-PARA-SEU-LINKEDIN]`
    * GitHub: `[LINK-PARA-SEU-GITHUB]`

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
