# Modelo de Elegibilidade de Crédito

Este repositório contém o modelo de classificação de elegibilidade de crédito baseado em K-Nearest Neighbors (KNN).

## 1. Tipo de Modelo

* **Algoritmo**: K-Nearest Neighbors (KNN) com  Neighbors = 30

## 2. Variáveis de Entrada

As variáveis utilizadas pelo modelo e a ordem no vetor de entrada são:

```
[salario_anual, historico_pagamento (score), credito_solicitado]
```

## 3. Exemplo de Previsão Real

* **Entrada (X)**: \[62149, 0.735597007642055, 16472]
* **Saída (y)**: \[2]

Nesse exemplo, o valor de saída `2` corresponde à categoria **Elegíveis com análise**.

## 4. Pré-processamento (Scaler)

* **Scaler utilizado**: StandardScaler
* **Arquivo de dump**: `scaler`

## 5. Modelo Pré-treinado

* **Arquivo de dump do modelo**: `KNN-Elegibilidade_de_credito`

## 6. Mapeamento de Classes

As classes retornadas pelo modelo correspondem às categorias de elegibilidade:

| Classe | Categoria             |
| ------ | --------------------- |
| 1      | Não elegíveis         |
| 2      | Elegíveis com análise |
| 3      | Elegíveis             |

---

Para utilizar o modelo:

1. Carregue o scaler (`scaler`).
2. Aplique o scaler às variáveis de entrada na ordem correta.
3. Carregue o modelo KNN (`KNN-Elegibilidade_de_credito`).
4. Execute `predict(X)` para obter a classe de elegibilidade.
