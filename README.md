# Desafios Data Science Intelivix

Escolha UM dos testes abaixo. Quanto mais avançado o nível da sua escolha, maior sua pontuação.

Choose wisely.....


## Básico

No link a seguir, encontra-se uma base de dados sobre características de algumas flores mapeadas em um determinado tipo: http://archive.ics.uci.edu/ml/datasets/Iris

O desafio consiste em:

1. Criar uma base de treino (66% do total dos textos pertencentes a uma das duas categorias) e uma base de teste (os 34% restantes); Os textos devem ser distribuídos aleatoriamente em ambas as bases;
2. Criar um classificador capaz de categorizar em uma das três categorias presentes na base uma flor que não esteja na base de treinamento, através do fornecimento de suas características para o classificador.

Sobre a entrega:

1. Deve-se escolher 3 diferentes classificadores, treiná-los, testá-los e reportar os resultados, comparando-os e escolhendo o melhor, justificando a escolha.
2. Para as comparações, deve-se calcular uma matriz de confusão para cada classificador.
3. Evidentemente, outras métricas adicionais que, por ventura, sejam consideradas necessárias, podem ser utilizadas.
4. Os códigos e o relatório devem ser entregues em um ipython notebook, o qual deve ser auto-suficiente para ser executado (assumindo que o computador a executar possua todas as ferramentas necessárias instaladas).

Ferramenta sugerida: scikit-learn.


## Intermediário

No NLTK (Natural Language Toolkit), uma plataforma para desenvolvimento de aplicações voltada para Processamento de Linguagem Natural para Python, estão disponíveis alguns corpora com textos já classificados, taggeados, etc. Um deles, o corpus “Brown”, reune 500 textos de diferentes categorias.

O desafio consiste em:

1. Identificar as 2 categorias mais frequentes, extrair os textos pertencentes a cada uma dessas categorias;
2. Criar uma base de treino (66% do total dos textos pertencentes a uma das duas categorias) e uma base de teste (os 34% restantes); Os textos devem ser distribuídos aleatoriamente em ambas as bases;
3. Criar um classificador capaz de categorizar em uma das duas categorias um texto qualquer.

O treinamento deve possuir duas etapas:

1. Pré-processamento:
 1. Extrair tokens, eliminando pontuações, stopwords e realizando stemming (ou stemização) nos termos restantes;
 2. Os textos de treinamento, representados por listas dos tokens restantes, devem ser convertidos em uma matriz TF-IDF (Text Frequency – Inverse Document Frequency).
2. Classificação:
 1. Cada linha da matriz, que representa um documento da base de treinamento, deve ser apresentada a um classificador juntamente com sua categoria, de forma que ocorra o aprendizado.	

O teste do classificador deve seguir o mesmo raciocínio. Um detalhe importante é o cálculo da parte IDF do vetor de características formado a partir do texto em teste, que deve ser feito usando as “variáveis globais” do cálculo da matriz TF-IDF da base de treinamento.

Sobre a entrega:

1. Deve-se escolher 3 diferentes classificadores, treiná-los, testá-los e reportar os resultados, comparando-os e escolhendo o melhor, justificando a escolha.
2. Para as comparações, deve-se calcular uma matriz de confusão para cada classificador.
3. Evidentemente, outras métricas adicionais que, por ventura, sejam consideradas necessárias, podem ser utilizadas.
4. Os códigos e o relatório devem ser entregues em um ipython notebook, o qual deve ser auto-suficiente para ser executado (assumindo que o computador a executar possua todas as ferramentas necessárias instaladas).

Ferramentas sugeridas:

1. NLTK (pré-processamento – alguns dos passos estão implementados, outros não);
2. scikit-learn (classificação).


## Avançado

No NLTK (Natural Language Toolkit), uma plataforma para desenvolvimento de aplicações voltada para Processamento de Linguagem Natural para Python, estão disponíveis alguns corpora com textos já classificados, taggeados, etc. Um deles, o corpus “Brown”, reune 500 textos de diferentes categorias.

O desafio consiste em:

1. Identificar as 2 categorias mais frequentes, extrair os textos pertencentes a cada uma dessas categorias;
2. Criar uma base de treino (66% do total dos textos pertencentes a uma das duas categorias) e uma base de teste (os 34% restantes); Os textos devem ser distribuídos aleatoriamente em ambas as bases;
3. Criar um classificador capaz de categorizar em uma das duas categorias um texto qualquer.

O treinamento deve possuir duas etapas:

1. Pré-processamento:
 1. Extrair tokens, eliminando pontuações, stopwords e realizando stemming (ou stemização) nos termos restantes;
 2. Os textos de treinamento, representados por listas dos tokens restantes, devem ser convertidos em uma matriz TF-IDF (Text Frequency – Inverse Document Frequency).
2. Classificação:
 1. Cada linha da matriz, que representa um documento da base de treinamento, deve ser apresentada a um classificador juntamente com sua categoria, de forma que ocorra o aprendizado.	

O teste do classificador deve seguir o mesmo raciocínio. Um detalhe importante é o cálculo da parte IDF do vetor de características formado a partir do texto em teste, que deve ser feito usando as “variáveis globais” do cálculo da matriz TF-IDF da base de treinamento.

Sobre a entrega:

1. Deve-se escolher 3 diferentes classificadores que possuam hiperparâmetros para serem ajustados;
2. Para cada classificador, deve-se experimentar diferentes combinações dos valores dos seus hiperparâmetros e escolher o melhor ajuste para cada um;
3. Com os classificadores otimamente ajustados, deve-se treiná-los, testá-los e reportar os resultados, comparando-os e escolhendo o melhor, justificando a escolha. Deve-se também justificar as escolhas para os ajustes dos hiperparâmetros para cada classificador através de comparações;
4. Para as comparações, deve-se calcular uma matriz de confusão para cada classificador;
5. Evidentemente, outras métricas adicionais que, por ventura, sejam consideradas necessárias, podem ser utilizadas;
6. Os códigos e o relatório devem ser entregues em um ipython notebook, o qual deve ser auto-suficiente para ser executado (assumindo que o computador a executar possua todas as ferramentas necessárias instaladas).

Ferramentas sugeridas:
1. NLTK (pré-processamento – alguns dos passos estão implementados, outros não);
2. scikit-learn (classificação).
