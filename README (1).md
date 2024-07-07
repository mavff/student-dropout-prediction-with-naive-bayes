
# Student Dropout Prediction Using Naive Bayes

Este projeto visa prever a evasão escolar de estudantes usando o classificador Naive Bayes. O método se baseia na suposição de independência entre os atributos, sendo uma abordagem probabilística eficiente e de fácil implementação.

## Descrição do Método

### Passos Envolvidos:

1. **Coleta de Dados**: Coleta de dados sobre estudantes, incluindo desempenho acadêmico, registros de frequência, informações demográficas e outros atributos relevantes.

2. **Pré-processamento dos Dados**: Limpeza dos dados para lidar com valores ausentes, normalização ou padronização de atributos numéricos e codificação de variáveis categóricas.

3. **Seleção de Atributos**: Identificação dos atributos mais relevantes que influenciam a taxa de evasão escolar. Isso pode envolver análise estatística ou expertise no domínio.

4. **Treinamento do Modelo**:
   - **Cálculo das Probabilidades Prévias**: Determinação da probabilidade geral de evasão e não evasão dos estudantes.
   - **Cálculo da Verossimilhança**: Para cada atributo, cálculo da probabilidade de observar cada valor do atributo dado o rótulo da classe (evasão ou não evasão).
   - **Aplicação do Teorema de Bayes**: Combinação das probabilidades prévias e verossimilhanças para calcular a probabilidade posterior de um estudante evadir dado seus valores de atributos.

5. **Avaliação do Modelo**: Avaliação do desempenho do modelo usando métricas como acurácia, precisão, recall e F1-score em um conjunto de dados de teste. A validação cruzada também pode ser usada para garantir a robustez do modelo.

6. **Predição**: Para novos dados de estudantes, o modelo Naive Bayes treinado é usado para prever a probabilidade de evasão. Estudantes com probabilidade acima de um certo limiar podem ser sinalizados para intervenção.

7. **Estratégias de Intervenção**: Com base nas predições, desenvolver estratégias de intervenção direcionadas para apoiar estudantes em risco e reduzir as taxas de evasão.

### Vantagens:
- **Simplicidade e Eficiência**: Naive Bayes é fácil de implementar e computacionalmente eficiente, sendo adequado para grandes conjuntos de dados.
- **Interpretabilidade**: A natureza probabilística do modelo permite uma compreensão clara de quais fatores contribuem para o risco de evasão.

### Limitações:
- **Suposição de Independência**: A suposição de que os atributos são independentes pode não ser válida em conjuntos de dados educacionais, potencialmente afetando a acurácia do modelo.
- **Dependência de Atributos**: O desempenho pode degradar se houver fortes dependências entre os atributos.

## Fonte dos Dados

Os dados utilizados para este projeto são provenientes do [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/index.php).

## Como Usar

1. Clone este repositório: `git clone https://github.com/seuusuario/student-dropout-prediction.git`
2. Instale as dependências: `pip install -r requirements.txt`
3. Execute o script de treinamento: `python train_model.py`
4. Use o modelo treinado para fazer predições: `python predict.py`

## Dependências

As dependências do projeto estão listadas no arquivo `requirements.txt`.
