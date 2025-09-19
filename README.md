# Recomendacao_Por_Imagens

Conceito do Sistema

O objetivo: dado um conjunto de imagens (ex: roupas, capas de livros, produtos), o sistema consegue recomendar imagens visualmente similares.

Como funciona:

Extrair características das imagens

Transformamos cada imagem em vetor numérico (embedding) usando um modelo pré-treinado de deep learning, ex: ResNet50, VGG16, EfficientNet.

Armazenar embeddings

Cada imagem terá um vetor que representa seu conteúdo visual.

Guardamos em um array ou banco de dados.

Comparar similaridade

Para recomendar imagens, calculamos a distância entre embeddings (cosine similarity ou Euclidean distance).

Quanto menor a distância, mais visualmente similares.

Retornar recomendações

Para cada imagem de entrada, retornamos as top N imagens mais próximas.

⚡ Estrutura do Projeto
image_recommender/
│── images/             # pasta com imagens do dataset
│── embeddings.npy      # embeddings pré-computados
│── filenames.npy       # nomes dos arquivos correspondentes
│── compute_embeddings.py
│── recommend.py
