# Smart Resume Analyzer 🤖📄

Sistema de classificação de currículos usando Machine Learning. Classifica resumes em categorias profissionais (Advocate, Banking, Healthcare, IT, etc.) utilizando Random Forest e TF-IDF.

## 📋 Recursos
- ✅ Carregamento e limpeza de dados de currículos
- ✅ Balanceamento de dataset
- ✅ Vetorização de texto com TF-IDF
- ✅ Modelo Random Forest treinado
- ✅ Avaliação completa (Acurácia, Precision, Recall, F1-Score)
- ✅ Matriz de Confusão visualizada
- ✅ Função de predição para novos currículos
- ✅ Modelos salvos em pickle para inferência

## 🛠️ Tech Stack
- **Python 3.10+**
- **scikit-learn** - Modelo de Machine Learning
- **pandas** - Manipulação de dados
- **numpy** - Operações numéricas
- **matplotlib & seaborn** - Visualização
- **Jupyter** - Notebooks interativos

## 📦 Instalação

1. Clone o repositório:
```bash
git clone https://github.com/Barbaralampert97/smart-resume-analyzer.git
cd smart-resume-analyzer
```

2. Crie um ambiente virtual (opcional mas recomendado):
```bash
python -m venv venv
venv\Scripts\activate  # Windows
# ou
source venv/bin/activate  # Linux/Mac
```

3. Instale as dependências:
```bash
pip install -r requirements.txt
```

## 🚀 Uso

Abra o Jupyter Notebook:
```bash
jupyter notebook resume_classification_lab.ipynb
```

Execute as células para:
1. Carregar e explorar os dados
2. Balancear o dataset
3. Treinar o modelo
4. Avaliar performance
5. Fazer predições em novos currículos

### Exemplo de Predição:
```python
resume_text = "Your resume text here..."
category = predict_resume_category(resume_text)
print(f"Categoria: {category}")
```

## 📊 Métricas de Desempenho
O modelo é avaliado usando:
- **Acurácia** - Percentual geral de acertos
- **Precision** - Confiabilidade das predições
- **Recall** - Capacidade de encontrar todos os casos
- **F1-Score** - Média harmônica entre Precision e Recall
- **Matriz de Confusão** - Visualização dos erros por categoria

## 📁 Estrutura do Projeto
```
resume-analyzer/
├── resume_classification_lab.ipynb              # Notebook principal com todo o pipeline
├── requirements.txt                             # Dependências do projeto
├── README.md                                    # Este arquivo
├── models/
│   ├── rf_classifier_categorization.pkl         # Modelo Random Forest treinado
│   └── tfidf_vectorizer_categorization.pkl      # Vetorizador TF-IDF
├── clean_resume_data.csv                        # Dados de treino limpos
├── jobs_dataset_with_features.csv               # Dataset original
└── *.txt                                        # Arquivos de amostra
```

## 📚 Dataset
Fonte: [Kaggle - Resume Datasets](https://www.kaggle.com/datasets/noorsaeed/resume-datasets/data?select=jobs_dataset_with_features.csv)

Categorias: Advocate, Banking, Healthcare, IT e outras profissões

## 🔍 Próximos Passos (Melhorias Futuras)
- [ ] Validação cruzada com cross_val_score
- [ ] Grid Search para otimização de hiperparâmetros
- [ ] Análise de Feature Importance
- [ ] API REST para inferência
- [ ] Interface web (Streamlit/Flask)
- [ ] Tratamento de mais categorias profissionais

## 👤 Autor
Barbara Lampert

## 📝 Licença
MIT License
