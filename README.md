# Tech Challenge - Classificação de Câncer de Mama

## 📋 Descrição do Projeto

Este projeto desenvolve um modelo de classificação para prever se um tumor é **maligno** ou **benigno** usando o dataset Breast Cancer Wisconsin. O notebook implementa e compara dois algoritmos de machine learning (Regressão Logística e K-Nearest Neighbors), além de utilizar técnicas de interpretabilidade com SHAP para entender as previsões do modelo.

## 🎯 Objetivos

- Carregar e preparar o dataset Breast Cancer Wisconsin
- Treinar modelos de classificação (Regressão Logística e KNN)
- Avaliar e comparar o desempenho dos modelos
- Interpretar os resultados usando SHAP values
- Identificar as features mais importantes para o diagnóstico

## 📊 Métricas de Desempenho

O projeto avalia os modelos usando:
- **Accuracy** (Acurácia)
- **Recall** (Sensibilidade) - crucial para minimizar falsos negativos
- **F1-Score** - equilíbrio entre precisão e recall
- **ROC-AUC** - capacidade de discriminação entre classes

## 🛠️ Tecnologias Utilizadas

- Python 3.x
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- SHAP

## 📁 Estrutura do Projeto

```
tech_challenge_1/
├── data.csv                    # Dataset Breast Cancer Wisconsin
├── tech_challenge.ipynb        # Notebook principal com análises
└── README.md                   # Este arquivo
```

## 🚀 Como Executar o Projeto

### Pré-requisitos

- Python 3.7 ou superior instalado
- Jupyter Notebook ou JupyterLab instalado

### Instalação das Dependências

1. Clone ou baixe este repositório
2. Navegue até o diretório do projeto:

```bash
cd tech_challenge_1
```

3. Instale as bibliotecas necessárias:

```bash
pip install pandas numpy scikit-learn matplotlib shap
```

Ou, se preferir usar um arquivo de requisitos:

```bash
pip install -r requirements.txt
```

*(Crie um arquivo `requirements.txt` com o seguinte conteúdo):*

```
pandas>=1.3.0
numpy>=1.21.0
scikit-learn>=1.0.0
matplotlib>=3.4.0
shap>=0.41.0
jupyter>=1.0.0
```

### Executando o Notebook

#### Opção 1: Jupyter Notebook (Local)

```bash
jupyter notebook tech_challenge.ipynb
```

Isso abrirá o notebook no seu navegador padrão.

#### Opção 2: JupyterLab (Local)

```bash
jupyter lab
```

Navegue até `tech_challenge.ipynb` na interface do JupyterLab.

#### Opção 3: Google Colab (Online)

1. Acesse [Google Colab](https://colab.research.google.com/)
2. Faça upload do arquivo `tech_challenge.ipynb`
3. Faça upload do arquivo `data.csv` para o ambiente Colab
4. Execute as células sequencialmente

### Executando o Código

1. Certifique-se de que o arquivo `data.csv` está no mesmo diretório do notebook
2. Execute as células do notebook sequencialmente (use `Shift + Enter` para executar cada célula)
3. A instalação do SHAP será feita automaticamente pela célula correspondente no notebook

## 📈 Principais Resultados

### Regressão Logística
- **Acurácia**: 97.37%
- **Recall**: 95.24%
- **F1-Score**: 96.39%
- **ROC-AUC**: 99.54%

### K-Nearest Neighbors (KNN)
- **Acurácia**: 95.61%
- **Recall**: 90.48%
- **F1-Score**: 93.83%
- **ROC-AUC**: 98.23%

## 🔍 Principais Insights

1. A **Regressão Logística** apresentou desempenho superior ao KNN em todas as métricas
2. O **Recall elevado** (95.24%) é crucial para minimizar falsos negativos em diagnósticos médicos
3. As features mais importantes para o diagnóstico incluem:
   - `texture_worst`
   - `radius_se`
   - `symmetry_worst`
   - `concave points_mean`

## ⚠️ Considerações Importantes

- Este modelo é uma **ferramenta de apoio à decisão**, não um substituto para avaliação médica profissional
- Recomenda-se validação clínica rigorosa antes de qualquer aplicação prática
- O modelo prioriza a detecção de casos malignos (alta sensibilidade) para minimizar riscos

## 📝 Licença

Este projeto é de uso educacional e acadêmico.

## 👥 Autor

Gabriel Dias

---

**Nota**: Para qualquer dúvida ou problema na execução, certifique-se de que todas as dependências estão instaladas corretamente e que o arquivo `data.csv` está no diretório correto.
