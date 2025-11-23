# 📝 Análise de Sentimentos em Resenhas de Livros (PLN em Português)

## 📌 Descrição do Projeto
Este projeto desenvolve um modelo de **Processamento de Linguagem Natural (PLN)** para classificar automaticamente resenhas de livros em português como **positivas** ou **negativas**.  
O objetivo é oferecer uma solução simples, eficiente e escalável, reduzindo a necessidade de análise manual em grandes volumes de texto.

O pipeline inclui:
- análise exploratória dos textos,
- pré-processamento (limpeza, normalização e remoção de stopwords),
- vetorização TF-IDF (unigramas e bigramas),
- treinamento de Regressão Logística,
- avaliação com métricas clássicas de classificação,
- testes manuais com frases novas.

---

## 👥 Integrantes
- **Maria Gabriela Barros** – RA: 10409037 – 10409037@mackenzista.com.br  
- **Raphaela Polonis** – RA: 10408843 – 10408843@mackenzista.com.br  
- **Felipe Carvalho** – RA: 10409804 – 104098043@mackenzista.com.br  
- **Bruno Gustavo Rocha** – RA: 10400926 – 10400926@mackenzista.com.br  

---

## 📊 Dataset Utilizado
**Amazon Brazilian Portuguese Books Reviews Dataset**  
Fonte: GitHub – Larissa Feliciana  
🔗 https://github.com/larifeliciana/books-reviews-portuguese

**Total de comentários:** 2000  
- **1000 positivos** (mais de 3 estrelas)  
- **1000 negativos** (menos de 3 estrelas)  

Formato:
- arquivos `.txt`,  
- cada linha representa uma resenha.

---

## 🛠️ Tecnologias e Ferramentas
- Python 3  
- Pandas  
- Scikit-learn  
- NLTK  
- Unidecode  
- Matplotlib  
- WordCloud  
- Jupyter Notebook / Google Colab  

---

## ⚙️ Modelo Utilizado
- **Vetorização:** TF-IDF (`ngram_range=(1,2)`, `min_df=2`)  
- **Algoritmo:** Regressão Logística  
- **Divisão:** 80% treino / 20% teste (estratificada)  
- **Pré-processamento:**  
  - remoção de acentos  
  - conversão para minúscculas  
  - remoção de pontuação  
  - remoção de stopwords  

---

## 📈 Resultados Obtidos
**Acurácia:** 0.88

### Relatório de Classificação
| Classe      | Precisão | Recall |
|-------------|----------|--------|
| Positivo    | 0.91     | 0.84   |
| Negativo    | 0.86     | 0.92   |

### Exemplos de Predições
- “Amei a história, personagens cativantes e final emocionante!” → **Positivo**  
- “Péssimo, confuso e cansativo. Não recomendo.” → **Negativo**  
- “Achei ok, mas esperava mais do enredo.” → **Negativo** *(zona limítrofe)*  

---

## ▶️ Como Executar o Projeto
1. Clone o repositório.  
2. Instale as dependências:  
   ```
   pip install -r requirements.txt
   ```
3. Coloque os arquivos:  
   - `books_pt_pos.txt`  
   - `books_pt_neg.txt`  
   no diretório raiz do projeto.  
4. Execute o notebook:  
   - `analise_exploratoria.ipynb`

---

## 📚 Referências
- FELICIANA, Larissa. *Amazon Brazilian Portuguese Books Reviews Dataset*. GitHub, 2020.  
- BIRD, Steven; KLEIN, Ewan; LOPER, Edward. *Natural Language Processing with Python*. O’Reilly Media, 2009.  
- JURAFSKY, Daniel; MARTIN, James H. *Speech and Language Processing*. 3rd ed., 2023.  
