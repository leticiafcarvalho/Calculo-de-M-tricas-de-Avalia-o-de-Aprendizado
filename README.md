```markdown
# Projeto de Avaliação de Desempenho de Modelos de Classificação

Este projeto tem como objetivo calcular as principais métricas para avaliação de modelos de classificação de dados.
As métricas incluem Acurácia, Sensibilidade (Recall), Especificidade, Precisão e F-Score.
Além disso, também é gerada a Curva ROC (Receiver Operating Characteristic) com a área sob a curva (AUC) para avaliar o desempenho do modelo.

## Funcionalidades

- **Cálculo das Métricas de Avaliação**: 
  O código calcula as métricas de avaliação de desempenho do modelo, incluindo:
  - **Acurácia**
  - **Sensibilidade (Recall)**
  - **Especificidade**
  - **Precisão**
  - **F-Score**

- **Curva ROC**:
  O código gera a **Curva ROC** (Receiver Operating Characteristic) e calcula a área sob a curva (**AUC**).
Essa curva é útil para avaliar a capacidade de classificação binária do modelo, indicando o quão bem o modelo separa as classes.

## Requisitos

- **Python** 3.x
- **Bibliotecas**:
  - `matplotlib`
  - `numpy`
  - `scikit-learn`

Você pode instalar as dependências com o seguinte comando:

```bash
pip install matplotlib numpy scikit-learn
```

## Como Usar

1. **Substitua os Dados de Entrada**:
   No exemplo fornecido, você pode substituir as variáveis `y_true` (rótulos reais) e `y_pred_prob` (probabilidades previstas) pelos dados reais do seu modelo de classificação.

2. **Exemplo de Dados**:
   O código inclui dados de exemplo, mas você pode facilmente adaptá-lo para os seus próprios dados. As variáveis `y_true` e `y_pred_prob` devem ser listas ou arrays:
   - `y_true`: Lista de rótulos verdadeiros (0 ou 1).
   - `y_pred_prob`: Lista de probabilidades previstas para a classe positiva (0 a 1).

3. **Executando o Código**:
   Execute o código Python para calcular as métricas de avaliação e gerar o gráfico ROC. O código calculará as métricas e exibirá o gráfico da curva ROC com a área sob a curva.

4. **Visualização**:
   O código usa a biblioteca **matplotlib** para plotar a Curva ROC e exibir o gráfico.

## Exemplo de Execução

Com os seguintes dados de entrada:

```python
y_true = [0, 1, 1, 0, 1, 0, 1, 0, 1, 1]  # Rótulos verdadeiros
y_pred_prob = [0.1, 0.8, 0.7, 0.2, 0.9, 0.4, 0.85, 0.6, 0.95, 0.3]  # Probabilidades previstas
```

O código calculará as métricas de avaliação:

```
Métricas de Avaliação:
Acurácia: 0.8000
Sensibilidade (Recall): 0.9091
Especificidade: 0.8000
Precisão: 0.8333
F-Score: 0.8696
```

Além disso, gerará o gráfico da Curva ROC com a área sob a curva **AUC**.

   ```markdown
   ## Fórmulas das Métricas

   As fórmulas utilizadas para calcular as métricas de avaliação são as seguintes:

   - **Acurácia**:  
     `Acurácia = (VP + VN) / (VP + VN + FP + FN)`

   - **Sensibilidade (Recall)**:  
     `Sensibilidade = VP / (VP + FN)`

   - **Especificidade**:  
     `Especificidade = VN / (VN + FP)`

   - **Precisão**:  
     `Precisão = VP / (VP + FP)`

   - **F-Score**:  
     `F-Score = 2 × (Precisão × Sensibilidade) / (Precisão + Sensibilidade)`
   ```

Onde:
- **VP**: Verdadeiros Positivos
- **VN**: Verdadeiros Negativos
- **FP**: Falsos Positivos
- **FN**: Falsos Negativos

## Contribuições

Se você quiser contribuir para este projeto, fique à vontade para abrir uma *issue* ou enviar um *pull request*. Agradecemos qualquer contribuição!
