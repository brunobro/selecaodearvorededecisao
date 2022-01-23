# Seleção de árvore de decisão do Ensemble Random Forest
Neste tutorial aprenderemos como selecionar a Árvore de Decisão mais simples a partir daquelas obtidas pelo emprego do algoritimo Random Forest.

**Porque utilizar Árvores de Decisão no Aprendizado de Máquina?**

**Vantagens das Árvores de Decisão**

1.   Requerem menos esforço para a preparação dos dados durante o pré-processamento: 
  * Não requer normalização de dados
  * Não exige dimensionamento de dados.
  * Trabalha tanto em dados caregóricos quanto numéricos.
2.   Valores ausentes não afetam o processo de construção do modelo de forma considerável.
3.   Os modelos são muito intuitivos.
4.   Os algoritimos possibilitam seleção de atributos (features).

**Desvantagens das Árvores de Decisão**

1.   Pequenas mudanças nos dados podem causar uma grande mudança na estrutura do modelo. Portanto, está sujeita a ruídos.
2.   Os modelos são propensos a superajustar (overfitting) aos dados. Isso acarreta em alta variância reduzindo a precisão.
3. Inadequada para base de dados muito grandes, pois tenderá a criar Árvores muito complexas, acarretando no overfitting.

**Random Forest (Florestas Aleatórias)**

Para driblar as desvantagens das Árvores de Decisão, foi proposto o algoritmo Random Forest. Basicamente, ele consiste em gerar vários modelos, evitando assim o overfitting. (Link para o artigo inicial: https://link.springer.com/article/10.1023/A:1010933404324)

*Entretanto, ao gerar vários modelos, como podemos continuar tendo em mãos o poder explicativo das árvores de decisão.*

Uma maneira de fazer isto é selecionar os modelos gerados. Mas não devemos selecionar qualquer modelo, pois estamos vizando a explicação do modelo aprendido. Portanto, devemos escolher o modelo mais simples.
