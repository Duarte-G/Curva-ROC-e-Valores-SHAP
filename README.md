# A Conexão entre Curva ROC e Valores SHAP
Este repositório contém exemplos de análise de desempenho de modelos de classificação usando a Curva ROC e explicações com valores SHAP, com base no Titanic Dataset.

**Curva ROC** <br>
A Curva ROC é um gráfico que mostra a relação entre a Taxa de Verdadeiros Positivos (Sensibilidade) e a Taxa de Falsos Positivos. Ela é usada para avaliar o desempenho de um modelo em diferentes limiares de classificação. A Área Sob a Curva (AUC) indica o quão bem o modelo consegue discriminar entre as classes:
- AUC = 1: modelo perfeito.
- AUC = 0.5: modelo aleatório.
- AUC < 0.5: desempenho pior que o aleatório.
No exemplo com o Titanic Dataset, a AUC foi 0,84, mostrando que o modelo tem um bom desempenho.
<p align="center">
  <img src="https://github.com/user-attachments/assets/7bc79d58-fa07-406a-8066-82905d6909d3">
</p>

**Valores SHAP** <br>
Os valores SHAP atribuem a cada feature uma contribuição proporcional ao impacto que ela tem nas previsões. Eles permitem visualizar quais variáveis foram mais influentes na decisão final, tanto para previsões individuais quanto para o comportamento geral do modelo.
<p align="center">
  <img src="https://github.com/user-attachments/assets/ff995ce5-37a2-4ca3-a2d7-5fe71003d6b1">
</p>
- Cores: Vermelho indica valores altos, enquanto azul indica valores baixos para cada feature. <br>
- Eixo X: Representa o impacto de cada variável na previsão final. Valores positivos aumentam a probabilidade de uma determinada classe (por exemplo, sobreviver), enquanto valores negativos a diminuem.
Neste caso, o sexo é a variável mais relevante: homens (valores altos, em vermelho) têm menor chance de sobreviver, enquanto mulheres (valores baixos, em azul) têm maior chance de sobrevivência.

<p><br></p>

**Conexão entre Curva ROC e SHAP** <br>
Enquanto a Curva ROC mede o desempenho geral do modelo em discriminar entre as classes, ela não revela quais atributos foram mais importantes no processo de tomada de decisão. Já os valores SHAP fornecem uma explicação detalhada sobre como o modelo usa cada feature para gerar suas previsões. <br>
Portanto, a Curva ROC mostra o desempenho global, e os valores SHAP explicam como esse desempenho é alcançado, detalhando a importância de cada variável na tomada de decisão do modelo.

## Como Usar
 - Clone o repositório para sua máquina local.
 - Instale as bibliotecas necessárias no código.
 - Execute o .ipynb para explorar o código e resultados.
 - Sinta-se à vontade para modificar a base de dados e ajustar o código para analisar diferentes conjuntos de dados.
