
# 📊 Análise e Previsão de Séries Temporais com Prophet

Projeto prático desenvolvido durante o curso **"Data Science: Analisando e prevendo séries temporais"**. O objetivo deste repositório é aplicar técnicas completas de ciência de dados para limpeza, análise exploratória, testes de hipóteses estatísticas, tratamento de outliers e modelagem preditiva de demanda de aluguel de bicicletas utilizando a biblioteca **Prophet** (Meta).

---

## 🎯 Objetivos do Projeto

* **Limpeza e Tratamento de Dados:** Identificação e remoção de registros duplicados e preenchimento de valores ausentes via interpolação linear.
* **Análise Exploratória de Dados (EDA):** Visualização da distribuição das variáveis climáticas e de demanda, identificando padrões e correlações.
* **Testes de Hipóteses Estatísticas:** Formulação e validação de hipóteses utilizando testes não paramétricos (Mann-Whitney U).
* **Análise de Séries Temporais:** Identificação de tendências e sazonalidades ao longo do tempo.
* **Modelagem Preditiva:** Construção, treinamento e avaliação de modelos de previsão utilizando a biblioteca **Prophet**.
* **Tratamento de Outliers e Avaliação:** Detecção e mitigação de valores atípicos para aprimorar a performance do modelo, avaliada por métricas como o **RMSE** (Root Mean Squared Error).

---

## 🗂️ Estrutura do Repositório

* `Series_temporais_com_Prophet.ipynb`: Notebook principal contendo todo o pipeline de análise, testes estatísticos, visualizações e modelagem preditiva.
* `bicicletas.csv`: Base de dados utilizada no projeto, contendo registros horários de contagem de bicicletas alugadas e variáveis meteorológicas/temporais (`data_hora`, `contagem`, `temperatura`, `sensacao_termica`, `umidade`, `velocidade_vento`, `clima`, `feriado`, `fim_de_semana`, `estacao`).

---

## 🛠️ Tecnologias e Bibliotecas Utilizadas

* **Python 3**
* **Pandas & NumPy:** Manipulação, limpeza e tratamento numérico dos dados.
* **Matplotlib & Seaborn:** Criação de gráficos exploratórios (histogramas, gráficos de dispersão, séries temporais).
* **SciPy (`mannwhitneyu`):** Realização de testes de hipóteses estatísticas.
* **Prophet:** Modelagem e previsão de séries temporais.
* **Scikit-Learn (`mean_squared_error`):** Cálculo de métricas de erro e validação do modelo.

---

## 🚀 Etapas Desenvolvidas no Notebook

1. **Preparação e Processamento:** Carregamento dos dados (`17.429` registros iniciais), tratamento de valores nulos nas colunas `temperatura` e `sensacao_termica` com interpolação linear e remoção de `15` linhas duplicadas.
2. **Exploração de Dados:** Análise descritiva (`describe()`) e visualizações gráficas relacionando condições climáticas (temperatura, sensação térmica, umidade e velocidade do vento) com o volume de aluguéis.
3. **Validação Estatística:** Aplicação de testes de hipóteses para verificar diferenças significativas na demanda em diferentes cenários (ex: dias úteis vs. fins de semana/feriados).
4. **Previsão com Prophet:** Ajuste do modelo temporal, geração de previsões futuras, interpretação dos componentes de tendência/sazonalidade e análise interativa dos resultados.
5. **Refinamento:** Tratamento de *outliers* para melhorar a precisão das estimativas e comparação dos resultados antes e depois da limpeza.

---

## 💻 Como Executar

1. **Via Google Colab (Recomendado):** Clique no botão **"Open in Colab"** no topo deste README para abrir e executar o notebook diretamente no navegador sem precisar configurar ambiente local.
2. **Localmente:**
```bash
git clone https://github.com/VictorGMSS/Analisando_e_Prevendo_Series_Temporais.git
cd Analisando_e_Prevendo_Series_Temporais
pip install pandas numpy matplotlib seaborn scipy prophet scikit-learn jupyter
jupyter notebook Series_temporais_com_Prophet.ipynb

```



---

## 👨‍💻 Informações pessoais

Victor Gabriel Martins e Souza

* 💼 LinkedIn: [https://www.linkedin.com/in/victorgms](https://www.linkedin.com/in/victorgms)
* 🌐 Portfólio: [https://verxstech.vercel.app](https://verxstech.vercel.app)
