# Projeto-IA

📌 Descrição do Projeto

Este projeto tem como objetivo desenvolver um modelo de Processamento de Linguagem Natural (PLN) capaz de classificar automaticamente comentários de usuários em português como positivos ou negativos.
A proposta é reduzir a necessidade de análise manual, que é trabalhosa em grande escala, e oferecer uma solução simples, eficiente e replicável.

👥 Integrantes

 - Maria Gabriela Barros – RA: 10409037 – 10409037@mackenzista.com.br
 - Raphaela Polonis – RA: 10408843 – 10408843@mackenzista.com.br
 - Felipe Carvalho – RA: 1049804 – 104098043@mackenzista.com.br
 - Bruno Gustavo Rocha – RA: 10400926 – 10400926@mackenzista.com.br
📊 Dataset Utilizado

Foi utilizado o Amazon Brazilian Portuguese Books Reviews Dataset, disponível em:
🔗 GitHub – Larissa Feliciana https://github.com/larifeliciana/books-reviews-portuguese

Total de comentários: 2000

1000 positivos (mais de 3 estrelas)

1000 negativos (menos de 3 estrelas)

Formato: arquivos .txt, cada linha representa um comentário.

🛠️ Tecnologias Utilizadas

Python 3

Pandas

Scikit-learn

Matplotlib

WordCloud

Jupyter Notebook / Google Colab

📈 Resultados Obtidos

Acurácia: 0.88

Relatório de classificação:

Positivo → Precisão 0.91 / Recall 0.84

Negativo → Precisão 0.86 / Recall 0.92

Exemplos de predições manuais:

“Amei a história, personagens cativantes e final emocionante!” → Positivo

“Péssimo, confuso e cansativo. Não recomendo.” → Negativo

“Achei ok, mas esperava mais do enredo.” → Negativo (limite entre neutro/negativo)

📚 Referências

FELICIANA, Larissa. Amazon Brazilian Portuguese Books Reviews Dataset. GitHub, 2020. Disponível em: https://github.com/larifeliciana/books-reviews-portuguese
. Acesso em: 28 set. 2025.

BIRD, Steven; KLEIN, Ewan; LOPER, Edward. Natural Language Processing with Python. O’Reilly Media, 2009.

JURAFSKY, Daniel; MARTIN, James H. Speech and Language Processing. 3rd ed. Draft, 2023.
