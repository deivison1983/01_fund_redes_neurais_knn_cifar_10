# Classificação de Imagens com k-Nearest Neighbors (kNN) utilizando o CIFAR-10

## Sobre o projeto

Implementação manual de um classificador k-Nearest Neighbors (kNN) com três abordagens de cálculo de distância, aplicado à classificação de imagens do dataset **CIFAR-10.**

Embora o kNN seja um algoritmo clássico de Machine Learning e não uma Rede Neural Artificial, seu estudo é fundamental para compreender conceitos essenciais de reconhecimento de padrões, classificação supervisionada e avaliação de modelos, que servem como base para algoritmos mais avançados de Deep Learning.

Este notebook faz parte de uma coleção de exercícios desenvolvidos durante minha **Pós-Graduação em Inteligência Artificial e Aprendizado de Máquina**.

Mais do que implementar um algoritmo específico, o objetivo é consolidar os fundamentos matemáticos, estatísticos e computacionais que sustentam o desenvolvimento de soluções modernas em Machine Learning e Deep Learning.

---

## Visão geral

O foco principal é a compreensão profunda do algoritmo k-Nearest Neighbors (kNN). Diferente de simplesmente chamar uma função pronta de uma biblioteca, este projeto foi concebido para solidificar os fundamentos teóricos do algoritmo. 

A implementação é feita em três estágios de complexidade computacional:

1. Força Bruta (Dois Laços): Implementação ingênua para entender o fluxo do algoritmo.

2. Vetorização Parcial (Um Laço): Utilização do numpy para otimizar uma das iterações.

3. Vetorização Total (Sem Laços): Implementação completamente vetorizada para máxima eficiência.

O projeto também explora a seleção de hiperparâmetros através de validação cruzada, uma etapa crucial para construir modelos que generalizam bem.

---

## Objetivos do Projeto

- Implementar um classificador k-Nearest Neighbors.
- Compreender o pipeline completo de classificação de imagens.
- Explorar diferentes estratégias para cálculo de distâncias.
- Avaliar o impacto do parâmetro **k** na acurácia do modelo.
- Aplicar técnicas de vetorização para otimização computacional.
- Desenvolver uma base sólida para estudos posteriores em Redes Neurais Convolucionais (CNNs).

---

## Dataset

O projeto utiliza o **CIFAR-10**, uma das bases mais tradicionais para estudos em Visão Computacional.

O conjunto contém:

- 60.000 imagens coloridas
- 10 categorias distintas
- Imagens com resolução de 32 × 32 pixels

Entre as classes presentes encontram-se aviões, automóveis, pássaros, gatos, cervos, cães, sapos, cavalos, navios e caminhões.

---

## Conceitos de Inteligência Artificial abordados

Durante o desenvolvimento deste exercício foram explorados diversos fundamentos importantes de Machine Learning:

- Aprendizado supervisionado
- Classificação de imagens
- Distância Euclidiana entre vetores
- Algoritmo k-Nearest Neighbors (kNN)
- Seleção do parâmetro k
- Processo de votação entre vizinhos
- Avaliação de desempenho por acurácia
- Preparação e organização dos dados
- Otimização computacional por vetorização
- Comparação entre diferentes implementações do algoritmo

---

## Principais Aprendizados e Diferenciais

O grande valor deste projeto está em "levantar o capô" do algoritmo.

Os principais pontos de aprendizado são:

* **Implementação Matemática do kNN:** A distância Euclidiana (L2) foi implementada manualmente (com np.sqrt, np.sum e np.square), demonstrando o entendimento da fórmula por trás da similaridade entre vetores de características (imagens achatadas).

* **Otimização de Desempenho com NumPy:** A comparação direta entre as três implementações (two_loops, one_loop, no_loops) não só mostra a importância da vetorização, mas também ensina na prática como o NumPy pode acelerar operações em ordens de magnitude.

* **Validação Cruzada:** A técnica de k-fold cross-validation foi implementada para determinar o melhor hiperparâmetro *k* (número de vizinhos), evitando overfitting e garantindo que a escolha do modelo seja mais robusta.

* **Visualização de Matriz de Distâncias:** A visualização da matriz de distância forneceu insights visuais sobre quais imagens (de treino e teste) são atípicas, um aprendizado importante sobre a natureza dos dados.

---

## Relação com Redes Neurais

Embora este projeto utilize o algoritmo kNN, ele faz parte da construção dos conhecimentos necessários para o estudo de Redes Neurais Artificiais.

Os conceitos desenvolvidos nesta atividade são utilizados posteriormente em arquiteturas mais sofisticadas, como:

- Redes Neurais Multicamadas (MLP)
- Redes Neurais Convolucionais (CNN)
- Deep Learning para Visão Computacional

Compreender o comportamento de modelos clássicos permite comparar desempenho, entender limitações e interpretar os ganhos obtidos com modelos neurais modernos.

---

## Tecnologias Utilizadas

- Python
- NumPy
- Matplotlib
- CIFAR-10
- Jupyter Notebook

---

## Aplicações

Os conhecimentos desenvolvidos neste projeto possuem aplicações em diversos problemas reais, incluindo:

- Classificação automática de imagens
- Sistemas de reconhecimento visual
- Visão Computacional
- Benchmark de algoritmos de classificação
- Estudos comparativos entre modelos clássicos e Deep Learning

---

## Resultados e Conclusões

A validação cruzada indicou que k=10 é o melhor valor, alcançando uma acurácia de aproximadamente 28.2% no conjunto de teste (com uma amostra reduzida de 5000/500 imagens para eficiência).

A análise de desempenho mostrou uma aceleração de mais de 75x na implementação completamente vetorizada (no_loops) em comparação com a versão de dois laços, destacando a importância crítica da otimização de código em projetos de Ciência de Dados.

A acurácia do kNN no CIFAR-10 (subamostrado) é baixa, o que já era esperado. Este resultado serve como um excelente baseline e reforça a necessidade de modelos mais complexos (como Redes Neurais) para problemas de visão computacional, um aprendizado fundamental para a pós-graduação.

---

## Autor

Deivison Morais. Visite o meu portfólio de projetos [aqui.](https://deivison1983.github.io/portfolio_projetos/)

Pós-Graduação em Inteligência Artificial e Aprendizado de Máquina - PUC Minas

Professor Orientador: Zenilton Patrocínio Jr.

### Contatos

<div>
  <a href = "https://www.linkedin.com/in/deivisonmorais/"><img src = "https://img.shields.io/badge/-deivisonmorais-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
  <a href = "mailto:deivison1983@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white"></a>
</div>
