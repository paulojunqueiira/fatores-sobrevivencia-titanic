# Análise de Sobrevivência no Titanic

### 1. Contexto e Questão

Este projeto tem como objetivo principal analisar os fatores que influenciaram a sobrevivência dos passageiros do naufrágio do Titanic. Compreender esses fatores pode fornecer insights históricos e demonstrar habilidades em análise de dados. As perguntas-chave a serem respondidas são:
* Quais características dos passageiros (sexo, classe social, idade, etc.) tiveram maior impacto na taxa de sobrevivência?
* Existe alguma relação entre o custo da passagem e a sobrevivência?
* O porto de embarque influenciou a taxa de sobrevivência?

### 2. Fonte de Dados

Utilizei o famoso conjunto de dados do Titanic, disponível publicamente, contendo informações sobre cada passageiro, incluindo:
* **Dados Pessoais:** ID do passageiro, nome, sexo, idade.
* **Informações da Viagem:** Classe da passagem, número de irmãos/cônjuges a bordo, número de pais/filhos a bordo, número do bilhete, custo da passagem, cabine, porto de embarque.
* **Resultado:** Indicador de sobrevivência (0 = Não, 1 = Sim).

### 3. Metodologia e Ferramentas

Para a condução desta Análise Exploratória de Dados (EDA), o projeto seguiu uma metodologia estruturada inspirada no Método P.C.T.A., garantindo o perfil, a limpeza e a transformação de todos os dados antes da análise final.

**Ferramentas: Python** (Google Colab) com foco exclusivo na biblioteca Pandas para todas as etapas de manipulação e análise.

1.  **Carregamento e Entendimento de Perfil (P):**
    * O conjunto de dados do Titanic foi carregado usando Pandas, com o PassengerId definido como índice para otimização e padronização.
    * Foi feita uma inspeção inicial para diagnosticar a qualidade dos dados (nulos, tipos e distribuição).

2.  **Pré-processamento e Limpeza (Fase C):**
    * As colunas foram renomeadas para português para facilitar a compreensão.
    * Colunas irrelevantes ou com excesso de nulos foram removidas, otimizando o tamanho do DataFrame.
    * O dataset foi consolidado através da imputação de dados faltantes (nulos), remoção de duplicatas e ajustes finais nos tipos de séries.

3.  **Engenharia de Features e Transformação (Fase T):**
    * Futuramente serão criados novos recursos para enriquecer o modelo de análise, como a variável Tamanho da Família e o agrupamento da variável contínua Idade em categorias.

4.  **Análise e Auditoria Final (A):**
    * O DataFrame final foi auditado para confirmar que não havia mais nulos e que todos os tipos de dados estavam corretos, garantindo a integridade da análise.

5.  **Visualização Interativa (Ferramenta de Visualização):**
    * Em um primeiro momento, o projeto não contemplou a utilização de ferramentas de visualização (como Power BI, Tableau ou bibliotecas gráficas como Matplotlib e Seaborn), pois o objetivo inicial foi praticar a análise exploratória de dados exclusivamente através da manipulação de DataFrames com a biblioteca Pandas. Visualizações gráficas serão adicionadas em versões futuras do projeto.

### 4. Principais Insights Encontrados

A análise revelou insights importantes sobre a sobrevivência no Titanic:
* **Sexo:** Mulheres tiveram uma taxa de sobrevivência significativamente maior do que homens (M: 82.62% x H: 12.93% - uma diferença de 69.69%).
* **Classe Social:** Passageiros em classes de passagem mais altas apresentaram maior taxa de sobrevivência. A classe 1 teve a maior taxa (57.59%), seguida pela classe 2 (42.24%) e, por último, a classe 3 (26.94%).
* **Sexo e Classe Social Combinados:** A combinação de sexo e classe social teve um impacto ainda mais notável, com mulheres na classe 1 apresentando a maior taxa de sobrevivência (97.92%), enquanto homens na classe 3 tiveram a menor (9.53%).
* **Idade:** Apesar de aproximadamente metade das Crianças (até 12 anos) terem sobrevivido, a taxa de sobrevivência (55.32%) foi maior do que a dos adultos (36.38%).
* **Parentesco:** Passageiros com familiares a bordo tiveram uma taxa de sobrevivência 1,29% maior (50.67%) do que passageiros que viajavam sozinhos (29.24%).
* **Custo da Passagem:** Passageiros que pagaram acima da média pelo bilhete tiveram uma taxa de sobrevivência maior (57.89%) do que aqueles que pagaram abaixo da média (31.64%).
* **Porto de Embarque:** A taxa de sobrevivência variou entre os portos de embarque, com passageiros que embarcaram em C (Cherbourg) apresentando a maior taxa (49.26%).

### 5. Resultado Final

A análise das taxas de sobrevivência por diferentes atributos fornece um panorama claro dos fatores que foram cruciais para determinar quem sobreviveu ao naufrágio do Titanic.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ze138eSNJkIvAGM0nFh0PBzAOjoF0_Wk?usp=sharing)
