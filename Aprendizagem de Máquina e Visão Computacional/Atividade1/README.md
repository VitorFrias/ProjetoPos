# Atividade de Aprendizagem de Máquina: Análise de Imagens com Python

Nesta atividade de aprendizagem de máquina, o objetivo foi analisar 15 imagens contendo parafusos e porcas, utilizando **Python** e técnicas de **processamento de imagens**. A tarefa principal era verificar se cada imagem possuía exatamente **10 parafusos e 10 porcas**. Caso a quantidade estivesse incorreta, o sistema deveria informar **quantos itens estavam faltando ou em excesso**.

## Etapas da Atividade

1. **Pré-processamento das Imagens**
   - Cada imagem foi convertida para **tons de cinza**.
   - Em seguida, foi aplicada uma **binarização** para facilitar a segmentação dos objetos.

2. **Identificação dos Objetos**
   - Após a binarização, utilizou-se técnicas de **rotulagem de componentes conectados** para identificar individualmente cada objeto presente na imagem.
   - Para classificar se o objeto era um parafuso ou uma porca, foram utilizados critérios baseados em:
     - **Área** do objeto.
     - **Dimensões** (altura e largura).

3. **Critérios de Classificação**
   - **Parafuso**: Área e pelo menos uma das dimensões (altura ou largura) acima de um determinado valor de referência.
   - **Porca**: Área superior a um valor mínimo, mas com dimensões inferiores às de um parafuso.

4. **Validação e Resultado**
   - O sistema contou quantos parafusos e porcas foram identificados na imagem.
   - Se a contagem de qualquer um dos itens fosse diferente de 10, o programa informava **quantos estavam faltando** ou a **quantidade excedente**.

## Tecnologias Utilizadas

- Linguagem: **Python**
- Bibliotecas principais:
  - `OpenCV` para processamento e análise das imagens
  - `NumPy` para manipulação de matrizes
  - `Matplotlib` para visualização dos resultados (opcional)

## Conclusão

A atividade demonstrou a eficácia de técnicas básicas de processamento de imagem na classificação e contagem de objetos em imagens reais. Além disso, reforçou a importância de definir corretamente os critérios de segmentação e classificação para garantir bons resultados em aplicações de visão computacional.

