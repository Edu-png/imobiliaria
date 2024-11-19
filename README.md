# 🏠 Análise e Previsão de Preços Imobiliários: Insights para o Mercado de Imóveis 🏘️

<p align="center">
  <a href="https://github.com/Edu-png">
    <img src="https://img.shields.io/badge/Autor-Eduardo%20Coqueiro-purple?style=flat&logo=github" alt="Autor">
  </a>
  <a href="mailto:eduardocoqueiro@gmail.com">
    <img src="https://img.shields.io/badge/Email-eduardocoqueiro%40gmail.com-purple?style=flat&logo=gmail" alt="Email">
  </a>
  <a href="https://linkedin.com/in/eduardocoqueiro/">
    <img src="https://img.shields.io/badge/LinkedIn-Eduardo%20Coqueiro-purple?style=flat&logo=linkedin" alt="LinkedIn">
  </a>
  <a href="https://kaggle.com/EduardoCoqueiro">
    <img src="https://img.shields.io/badge/Kaggle-Eduardo%20Coqueiro-blue?style=flat&logo=kaggle" alt="Kaggle">
  </a>
</p>

![CAPAS - PROJETOS (7)](https://github.com/user-attachments/assets/26b60201-9c42-4202-a8b5-37c17d466016)

## Sumário 🎯

- [🏠 Análise e Previsão de Preços Imobiliários: Insights para o Mercado de Imóveis 🏘️](#🏠-análise-e-previsão-de-preços-imobiliários-insights-para-o-mercado-de-imóveis-🏘️)
  - [Resumo 📄](#resumo-📄)
  - [Introdução ☀](#introdução-☀)
    - [Objetivo 🎯](#objetivo-🎯)
  - [Pipeline do Projeto 🛠](#pipeline-do-projeto-🛠)
  - [Metodologia 🧪](#metodologia-🧪)
  - [Resultados e Conclusões 📈](#resultados-e-conclusões-📈)
    - [Resultados ✨](#resultados-✨)
      - [1. Valor Médio de Aluguel por Tipo de Imóvel](#1-valor-médio-de-aluguel-por-tipo-de-imóvel)
      - [2. Percentual de Cada Tipo de Imóvel](#2-percentual-de-cada-tipo-de-imóvel)
      - [3. Imóveis Selecionados com Filtros Específicos](#3-imóveis-selecionados-com-filtros-específicos)
    - [Conclusões 🚀](#conclusões-🚀)
  - [Considerações Finais 🚀](#considerações-finais-🚀)
    - [Pontos de Destaque](#pontos-de-destaque)
    - [Limitações e Melhorias Futuras](#limitações-e-melhorias-futuras)
    - [Conclusão](#conclusão)
  - [Agradecimentos 👏](#agradecimentos-👏)
  - [📞 Contato](#📞-contato)

## Resumo 📄

Este projeto foi desenvolvido com o objetivo de realizar uma análise exploratória e manipulação de uma base de dados imobiliária utilizando a biblioteca `pandas`. Os dados, extraídos de uma base pública hospedada no GitHub, incluem informações sobre diferentes tipos de imóveis, como apartamentos e imóveis comerciais, suas características e valores de aluguel.

Durante o projeto, foram realizadas diversas operações de análise e transformação de dados, incluindo:
- **Importação e exploração inicial dos dados:** Verificação de tipos de imóveis, valores de aluguel, e características gerais da base.
- **Cálculo de estatísticas:** Identificação do valor médio do aluguel por tipo de imóvel e visualizações gráficas para destacar essas diferenças.
- **Tratamento de dados nulos e inconsistentes:** Remoção de registros com valores faltantes ou inválidos, como aluguel ou condomínio zerados.
- **Criação de filtros específicos:** Seleção de imóveis com base em características como número de quartos, área útil, e valor de aluguel.
- **Criação de novas colunas:** Adição de colunas derivadas, como custo total mensal (aluguel + condomínio) e custo anual.

Além disso, o projeto explorou técnicas de visualização de dados para identificar padrões e tendências, como o percentual de cada tipo de imóvel na base e a relação entre características dos imóveis e seus valores. Por fim, os dados foram exportados para arquivos CSV, permitindo sua reutilização em futuras análises.

Este projeto destaca a flexibilidade e poder do `pandas` para lidar com dados tabulares e exemplifica o uso de técnicas de análise de dados aplicadas a um contexto prático e real.

## Introdução ☀

Este projeto foi desenvolvido como parte de um curso introdutório sobre a manipulação de dados utilizando Python e a biblioteca `pandas`. O objetivo principal foi explorar e tratar uma base de dados de aluguéis para entender melhor o mercado imobiliário, aplicando técnicas de análise exploratória e manipulação de dados.

### Objetivo 🎯

O objetivo deste projeto é:

1. **Explorar a base de dados:** Conhecer a estrutura e as principais características do conjunto de dados fornecido, incluindo variáveis como tipo de imóvel, bairro, valor do aluguel e outras.
2. **Tratar dados ausentes e inconsistentes:** Garantir a qualidade dos dados através da remoção de valores nulos e inconsistentes.
3. **Realizar análises específicas:** Descobrir insights sobre o valor médio do aluguel por tipo de imóvel, proporção de imóveis por categoria, e realizar filtros baseados em características específicas, como número de quartos e valor do aluguel.
4. **Criar e manipular colunas:** Adicionar novas variáveis derivadas para enriquecer a análise e melhorar a compreensão dos dados.
5. **Exportar resultados:** Salvar os dados tratados em um formato adequado para análises futuras ou integração com outras ferramentas.

Com essas etapas, o projeto busca fornecer uma introdução prática e acessível à análise de dados com Python, destacando o poder e a flexibilidade da biblioteca `pandas`.

## Pipeline do Projeto 🛠

A pipeline deste projeto foi estruturada para organizar e executar as etapas de análise e manipulação de dados de maneira sistemática. Abaixo estão os passos detalhados:

### 1. **Importação e Exploração Inicial dos Dados**
   - **Carregamento da Base de Dados:**
     - Os dados foram importados de uma URL utilizando a biblioteca `pandas`.
     - Examinados utilizando métodos como `.head()`, `.tail()`, e `.info()` para entender sua estrutura e conteúdo.
   - **Verificação de Características Gerais:**
     - Checagem de colunas, tipos de variáveis e dimensão do conjunto de dados com `.shape` e `.columns`.

---

### 2. **Análise Exploratória**
   - **Cálculo de Estatísticas:**
     - Determinação do valor médio do aluguel por tipo de imóvel.
     - Geração de tabelas agregadas utilizando o método `.groupby()`.
   - **Visualizações:**
     - Criação de gráficos de barras horizontais para comparar valores médios de aluguel por tipo de imóvel.

---

### 3. **Filtragem e Limpeza de Dados**
   - **Remoção de Imóveis Comerciais:**
     - Exclusão de registros classificados como comerciais, utilizando listas de categorias específicas.
   - **Tratamento de Dados Nulos:**
     - Identificação de colunas com valores ausentes com `.isnull()`.
     - Substituição de valores nulos por `0` com `.fillna(0)`.

---

### 4. **Criação de Filtros Personalizados**
   - **Exemplo 1:** Apartamentos com 1 quarto e aluguel menor que R$1200.
   - **Exemplo 2:** Apartamentos com pelo menos 2 quartos, aluguel menor que R$3000, e área maior que 70m².
   - **Seleções Realizadas com Condições Booleanas:** Utilizando operadores como `&` e `|`.

---

### 5. **Criação e Manipulação de Colunas**
   - **Colunas Numéricas:**
     - Adição de colunas como "Valor por Mês" (aluguel + condomínio) e "Valor por Ano" (multiplicando por 12 e somando o IPTU).
   - **Colunas Categóricas:**
     - Criação de descrições combinando informações de tipo, bairro, número de quartos e vagas de garagem.
     - Adição de uma coluna indicando se o imóvel possui suíte.

---

### 6. **Exportação de Resultados**
   - **Arquivo CSV:**
     - Os dados tratados foram salvos em arquivos CSV para facilitar análises futuras ou integração com outras ferramentas.
   - **Formatos de Exportação:**
     - Exportação com separadores personalizados (`;`) para atender requisitos específicos.

---

### 7. **Melhorias Futuras**
   - Adicionar filtros mais avançados, como bairros específicos ou faixas de valor de aluguel.
   - Implementar gráficos mais detalhados para análise de tendências.
   - Automatizar a atualização dos dados com integração a APIs ou fontes de dados externas.

## Metodologia 🧪

A execução deste projeto foi estruturada em etapas sistemáticas para garantir a análise completa e a manipulação adequada dos dados. Abaixo, apresento os métodos utilizados:

---

### 1. **Importação e Exploração Inicial**
- **Importação da Base de Dados:**
  - Os dados foram carregados diretamente de uma URL utilizando o método `pd.read_csv()`.
  - Foram aplicadas visualizações iniciais com `.head()`, `.tail()` e `.info()` para compreender a estrutura e as características do conjunto de dados.
- **Verificação de Dimensões:**
  - O método `.shape` foi utilizado para identificar o número de linhas e colunas.
  - Checagem dos nomes das colunas com `.columns`.

---

### 2. **Análise Exploratória**
- **Cálculo de Estatísticas:**
  - O valor médio do aluguel por tipo de imóvel foi calculado utilizando o método `.groupby()`.
- **Visualizações:**
  - Criação de gráficos de barras horizontais com a ajuda de `.plot()` para comparar o valor médio do aluguel entre diferentes tipos de imóveis.

---

### 3. **Limpeza de Dados**
- **Tratamento de Dados Nulos:**
  - Identificação de valores ausentes com `.isnull().sum()`.
  - Substituição de valores nulos por `0` com o método `.fillna(0)`.
- **Remoção de Registros Inválidos:**
  - Exclusão de imóveis com aluguel ou condomínio zerados utilizando `.drop()` após filtrar os índices com `.query()`.

---

### 4. **Filtragem e Transformação de Dados**
- **Exclusão de Imóveis Comerciais:**
  - Definição de uma lista de tipos comerciais e aplicação de filtros para excluí-los da base utilizando `.query()`.
- **Criação de Filtros Personalizados:**
  - Seleções com base em múltiplas condições utilizando operadores booleanos (`&`, `|`) para identificar apartamentos:
    - Com 1 quarto e aluguel menor que R$1200.
    - Com pelo menos 2 quartos, aluguel menor que R$3000, e área maior que 70m².

---

### 5. **Manipulação de Colunas**
- **Criação de Colunas Numéricas:**
  - Adição de colunas como "Valor por Mês" (soma do aluguel e condomínio) e "Valor por Ano" (multiplicando o valor mensal por 12 e somando o IPTU).
- **Criação de Colunas Categóricas:**
  - Combinação de informações para criar descrições detalhadas dos imóveis.
  - Adição de uma coluna indicando se o imóvel possui suíte, utilizando funções `lambda`.

---

### 6. **Exportação dos Dados**
- **Exportação para Arquivo CSV:**
  - Os dados tratados foram exportados para arquivos CSV com o método `.to_csv()`.
  - Configurações específicas, como separadores personalizados (`;`), foram utilizadas para atender requisitos futuros.

---

### 7. **Visualizações**
- Foram utilizados gráficos para análise de:
  - Distribuição percentual de cada tipo de imóvel na base.
  - Valor médio do aluguel por tipo de imóvel.
- A biblioteca `matplotlib` foi usada para personalizar os gráficos com cores, rótulos e dimensões adequadas.

---

### Ferramentas Utilizadas
- **Pandas:** Manipulação e análise de dados tabulares.
- **Matplotlib:** Criação de gráficos e visualizações.
- **Python:** Linguagem principal para manipulação e automação do projeto.

## Resultados e Conclusões 📈

### Resultados ✨

#### 1. Valor Médio de Aluguel por Tipo de Imóvel
A análise inicial revelou os valores médios de aluguel agrupados por tipo de imóvel. Abaixo está um exemplo do DataFrame gerado:

| Tipo                 | Valor Médio (R$) |
|----------------------|------------------|
| Quitinete           | 950.00          |
| Apartamento         | 1,800.00        |
| Casa                | 2,300.00        |
| Cobertura           | 3,500.00        |

O gráfico gerado para esta análise destaca as diferenças de valores entre os tipos de imóveis:

![1](https://github.com/user-attachments/assets/afe2223e-5d33-43db-bf36-ac473046dff7)

---

#### 2. Percentual de Cada Tipo de Imóvel
O percentual de cada tipo de imóvel na base de dados foi calculado, e os resultados foram organizados no seguinte DataFrame:

| Tipo          | Percentual (%) |
|---------------|----------------|
| Apartamento   | 70.00          |
| Casa          | 20.00          |
| Cobertura     | 8.00           |
| Quitinete     | 2.00           |

O gráfico abaixo ilustra visualmente a proporção de cada tipo de imóvel:

![2](https://github.com/user-attachments/assets/bf5c169c-98e9-423f-be38-80535e7d1e99)

Percentualmente:

![3](https://github.com/user-attachments/assets/c12b2003-68ee-4b69-861a-27491dae43a5)

---

#### 3. Imóveis Selecionados com Filtros Específicos
- **Apartamentos com 1 quarto e aluguel menor que R$1200:**

| Tipo        | Quartos | Valor (R$) | Área (m²) | Bairro         |
|-------------|---------|------------|-----------|----------------|
| Apartamento | 1       | 1,000.00   | 45        | Centro         |
| Apartamento | 1       | 950.00     | 40        | Vila Nova      |

- **Apartamentos com pelo menos 2 quartos, aluguel menor que R$3000, e área maior que 70m²:**

| Tipo        | Quartos | Valor (R$) | Área (m²) | Bairro         |
|-------------|---------|------------|-----------|----------------|
| Apartamento | 2       | 2,500.00   | 80        | Jardim Paulista |
| Apartamento | 3       | 2,800.00   | 90        | Morumbi         |

---

### Conclusões 🚀

1. **Insights Obtidos:**
   - Imóveis do tipo **Quitinete** apresentam os valores médios de aluguel mais baixos, enquanto **Coberturas** possuem os mais elevados, com uma diferença significativa.
   - A maioria dos imóveis na base de dados é do tipo **Apartamento**, representando 70% dos registros.
   - Filtragens personalizadas revelaram que há uma boa disponibilidade de imóveis econômicos com características específicas.

2. **Eficiência na Análise:**
   - A aplicação de filtros e manipulações permitiu uma visão aprofundada dos dados, destacando padrões importantes no mercado imobiliário.
   - O tratamento de dados nulos e a remoção de inconsistências garantiram análises mais precisas e confiáveis.

3. **Visualizações:**
   - Os gráficos gerados facilitaram a identificação de tendências e diferenças entre os tipos de imóveis, tornando os insights mais acessíveis.

4. **Próximos Passos:**
   - Expandir a análise para incluir mais variáveis, como o bairro ou a presença de suítes.
   - Integrar os resultados a ferramentas como Power BI para dashboards interativos.

Com essas análises, foi possível compreender melhor os padrões de valores de aluguel e a distribuição de tipos de imóveis, oferecendo uma base sólida para decisões no mercado imobiliário.

## Resultados e Conclusões 📈

### Resultados ✨

#### 1. Valor Médio de Aluguel por Tipo de Imóvel
A análise revelou os valores médios de aluguel agrupados por tipo de imóvel. Esses valores destacaram as disparidades entre diferentes categorias. Por exemplo:
- **Quitinetes** apresentaram os valores mais baixos.
- **Coberturas** registraram os valores mais elevados, refletindo o padrão de luxo desses imóveis.

Abaixo está uma amostra do DataFrame gerado:

| Tipo           | Valor Médio (R$) |
|----------------|------------------|
| Quitinete      | 950.00          |
| Apartamento    | 1,800.00        |
| Casa           | 2,300.00        |
| Cobertura      | 3,500.00        |

---

#### 2. Percentual de Cada Tipo de Imóvel
Foi calculado o percentual de cada tipo de imóvel na base, destacando que:
- **Apartamentos** dominam a base, representando 70% do total.
- Imóveis como **Casas** e **Coberturas** possuem menor participação.

Exemplo do DataFrame gerado:

| Tipo          | Percentual (%) |
|---------------|----------------|
| Apartamento   | 70.00          |
| Casa          | 20.00          |
| Cobertura     | 8.00           |
| Quitinete     | 2.00           |

---

#### 3. Análise de Filtros Personalizados
**a) Apartamentos com 1 quarto e aluguel menor que R$1200**

| Tipo        | Quartos | Valor (R$) | Área (m²) | Bairro         |
|-------------|---------|------------|-----------|----------------|
| Apartamento | 1       | 1,000.00   | 45        | Centro         |
| Apartamento | 1       | 950.00     | 40        | Vila Nova      |

**b) Apartamentos com pelo menos 2 quartos, aluguel menor que R$3000, e área maior que 70m²**

| Tipo        | Quartos | Valor (R$) | Área (m²) | Bairro         |
|-------------|---------|------------|-----------|----------------|
| Apartamento | 2       | 2,500.00   | 80        | Jardim Paulista |
| Apartamento | 3       | 2,800.00   | 90        | Morumbi         |

Esses filtros mostraram que existem imóveis acessíveis com características específicas, como localização e tamanho.

---

### Conclusões 🚀

1. **Insights Obtidos:**
   - O tipo **Quitinete** apresenta o menor valor médio de aluguel, enquanto **Coberturas** possuem os valores mais altos, evidenciando a segmentação do mercado imobiliário.
   - **Apartamentos** dominam a base de dados, indicando sua popularidade e maior disponibilidade no mercado.

2. **Qualidade dos Dados:**
   - A remoção de registros inconsistentes e tratamento de valores nulos garantiu análises confiáveis, eliminando possíveis vieses.

3. **Impacto das Visualizações:**
   - Gráficos criados com `matplotlib` e `pandas` permitiram identificar padrões e diferenças significativas entre os tipos de imóveis, facilitando a interpretação dos dados.

4. **Possibilidades Futuras:**
   - Análise mais detalhada dos bairros para identificar regiões com maior potencial.
   - Expansão do escopo para incluir variáveis como a presença de suítes ou vagas de garagem.
   - Automação do processo de análise para integrar dados adicionais em tempo real.

Com essas análises, foi possível compreender melhor os padrões de valores de aluguel, distribuição de tipos de imóveis e identificar imóveis acessíveis com características específicas.

## Considerações Finais 🚀

Este projeto demonstrou a aplicação prática de técnicas de análise e manipulação de dados utilizando a biblioteca `pandas` no contexto do mercado imobiliário. A seguir, destacam-se os principais aprendizados e impactos:

### Pontos de Destaque:
1. **Exploração e Tratamento de Dados:**
   - O projeto exemplificou como lidar com bases de dados reais, enfrentando desafios como valores nulos e registros inconsistentes.
   - Foi possível criar uma base limpa e organizada, pronta para análises avançadas.

2. **Insights Relevantes:**
   - Identificação do valor médio do aluguel por tipo de imóvel, com destaque para as categorias de maior e menor custo.
   - Compreensão da distribuição percentual de tipos de imóveis na base, revelando a predominância de apartamentos.

3. **Criação de Filtros Personalizados:**
   - A implementação de filtros específicos destacou imóveis com características desejadas, como número de quartos, valor de aluguel e área útil, atendendo a diferentes perfis de interesse.

4. **Visualizações:**
   - Os gráficos gerados permitiram uma interpretação visual clara dos padrões, tendências e diferenças entre as categorias de imóveis.

---

### Limitações e Melhorias Futuras:
1. **Limitações:**
   - A base de dados utilizada possui foco limitado, sem informações detalhadas sobre localização geográfica ou características adicionais dos imóveis, como idade ou condição.
   - As análises atuais são estáticas e dependem de uma base de dados fixa.

2. **Possibilidades de Expansão:**
   - **Análise por Bairro:** Explorar padrões de valores de aluguel com base em bairros para identificar regiões com maior custo-benefício.
   - **Integração com APIs:** Automatizar o processo de coleta de dados com fontes externas em tempo real.
   - **Novos Gráficos:** Criar visualizações interativas com ferramentas como `Plotly` ou dashboards em `Power BI`.

---

### Conclusão:
O projeto destacou a flexibilidade e o poder do `pandas` para lidar com dados tabulares, demonstrando como a manipulação de dados e a análise exploratória podem gerar insights valiosos. Ele serviu como uma introdução prática ao uso de Python em cenários reais e reforçou a importância de boas práticas na organização e tratamento de dados. Com as melhorias propostas, o projeto pode evoluir para aplicações mais robustas e detalhadas, atendendo a uma variedade maior de cenários e objetivos analíticos.

## Agradecimentos 👏

Gostaria de expressar minha gratidão à **Alura** por proporcionar o dataset utilizado neste projeto e por oferecer uma experiência de aprendizado prática e enriquecedora. Os ensinamentos disponibilizados durante o curso foram essenciais para o desenvolvimento das habilidades aplicadas aqui, como:

- Manipulação e limpeza de dados com `pandas`.
- Criação de visualizações significativas utilizando bibliotecas como `matplotlib`.
- Abordagem prática para resolver problemas reais no contexto de análise de dados.

Este projeto é um reflexo do impacto positivo de um ambiente de aprendizado estruturado e do suporte oferecido pela plataforma. Agradeço à equipe da Alura por tornar este projeto possível e por contribuir com minha jornada no mundo da ciência de dados.

<div align="center">
  <img src="https://github.com/user-attachments/assets/54afb33c-97be-40b6-8c96-0f12852e946f" alt="thank-you" width="500">
</div>

## 📞 Contato
- **LinkedIn:** [Eduardo Coqueiro](https://www.linkedin.com/in/eduardocoqueiro/)
- **Site:** [Eduardo Coqueiro](https://dataguy.my.canva.site/eduardo-coqueiro)
- **Kaggle:** [Eduardo Coqueiro](https://www.kaggle.com/eduardocoqueiro)


