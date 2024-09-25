# A Conexão entre Curva ROC e Valores SHAP
Este repositório contém exemplos de análise de desempenho de modelos de classificação usando a Curva ROC e explicações com valores SHAP, com base no Titanic Dataset.

**Curva ROC** <br>
A Curva ROC é um gráfico que mostra a relação entre a Taxa de Verdadeiros Positivos (Sensibilidade) e a Taxa de Falsos Positivos. Ela é usada para avaliar o desempenho de um modelo em diferentes limiares de classificação. A Área Sob a Curva (AUC) indica o quão bem o modelo consegue discriminar entre as classes:
- AUC = 1: modelo perfeito.
- AUC = 0.5: modelo aleatório.
- AUC < 0.5: desempenho pior que o aleatório.
No exemplo com o Titanic Dataset, a AUC foi 0,85, mostrando que o modelo tem um bom desempenho.
<p align="center">
  <img src="https://github.com/user-attachments/assets/f7585064-37aa-4ba8-a3e2-69cfd05ee083">
</p>

**Valores SHAP** <br>
Os Valores SHAP explicam a contribuição de cada variável para a previsão. Eles mostram quais variáveis mais influenciam o modelo e se aumentam ou diminuem a probabilidade de uma classe. No exemplo com o Titanic Dataset, "Sex" (gênero) é a variável com maior impacto.
<p align="center">
  <img src="https://github.com/user-attachments/assets/e7cae3e6-cdf8-43e4-b730-8238048950e5">
</p>

**Conexão entre Curva ROC e SHAP** <br>
Enquanto a Curva ROC mede o desempenho geral do modelo em discriminar entre as classes, ela não revela quais atributos foram mais importantes no processo de tomada de decisão. Já os valores SHAP fornecem uma explicação detalhada sobre como o modelo usa cada feature para gerar suas previsões. <br>
Portanto, a Curva ROC mostra o desempenho global, e os valores SHAP explicam como esse desempenho é alcançado, detalhando a importância de cada variável na tomada de decisão do modelo.

## Como Usar
 - Clone o repositório para sua máquina local.
 - Instale as bibliotecas necessárias no código.
 - Execute o .ipynb para explorar o código e resultados.
 - Sinta-se à vontade para modificar a base de dados e ajustar o código para analisar diferentes conjuntos de dados.
