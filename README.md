# Análise de Sobrevivência no Titanic

### 1. Contexto e Problema de Negócio

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

Para conduzir a análise e responder às perguntas, o projeto seguiu um fluxo de trabalho em três etapas, utilizando as seguintes ferramentas:

1.  **Carregamento e Pré-processamento dos Dados (Python com Pandas):**
    * A primeira etapa foi carregar o conjunto de dados do Titanic usando a biblioteca **Pandas** no **Google Colab**.
    * As colunas foram renomeadas para português para facilitar a compreensão.
    * A coluna 'ticket' foi removida por não ser relevante para a análise de sobrevivência.

2.  **Análise Exploratória e Cálculo de Taxas de Sobrevivência (Python com Pandas):**
    * O **Pandas** foi utilizado para calcular as taxas de sobrevivência com base em diferentes atributos dos passageiros, como sexo, classe social, faixa etária (crianças vs. adultos), presença de familiares, custo da passagem (acima ou abaixo da média) e porto de embarque.
    * Foram gerados outputs de texto no notebook para apresentar as taxas de sobrevivência calculadas para cada categoria.

3.  **Visualização Interativa (Opcional - Ferramenta de Visualização):**
    * Embora a análise principal tenha sido apresentada em formato de texto, os dados poderiam ser exportados para uma ferramenta de visualização interativa (como Power BI, Tableau, etc.) para a criação de um painel mais dinâmico, permitindo filtros e exploração visual dos dados. Um placeholder para o link será incluído abaixo.

### 4. Principais Insights Encontrados

A análise revelou insights importantes sobre a sobrevivência no Titanic:
* **Sexo:** Mulheres tiveram uma taxa de sobrevivência significativamente maior do que homens.
* **Classe Social:** Passageiros em classes de passagem mais altas apresentaram maior taxa de sobrevivência. A classe 1 teve a maior taxa, seguida pela classe 2 e, por último, a classe 3.
* **Sexo e Classe Social Combinados:** A combinação de sexo e classe social teve um impacto ainda mais notável, com mulheres na classe 1 apresentando a maior taxa de sobrevivência, enquanto homens na classe 3 tiveram a menor.
* **Idade:** Crianças (até 12 anos) tiveram uma taxa de sobrevivência maior do que adultos.
* **Parentesco:** Passageiros com familiares a bordo tiveram uma taxa de sobrevivência maior do que passageiros que viajavam sozinhos.
* **Custo da Passagem:** Passageiros que pagaram acima da média pelo bilhete tiveram uma taxa de sobrevivência maior do que aqueles que pagaram abaixo da média.
* **Porto de Embarque:** A taxa de sobrevivência variou entre os portos de embarque, com passageiros que embarcaram em C (Cherbourg) apresentando a maior taxa.

### 5. Resultado Final

A análise das taxas de sobrevivência por diferentes atributos fornece um panorama claro dos fatores que foram cruciais para determinar quem sobreviveu ao naufrágio do Titanic.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ze138eSNJkIvAGM0nFh0PBzAOjoF0_Wk?usp=sharing)
