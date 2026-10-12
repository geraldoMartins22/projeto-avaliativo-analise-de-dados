# 📊 Projeto Avaliativo — Visualização de Dados de RH

---

# 👨‍💻 Autor

**Geraldo Martins Barros**

**Visualização de dados e Business Intelligence - Turma 3**

Projeto desenvolvido para fins acadêmicos e avaliativos, aplicando conhecimentos de **SQL, Python, Pandas, Análise Exploratória de Dados e visualização de dados**.

---

## 📌 Sobre o projeto

Este projeto foi desenvolvido como parte do Projeto Avaliativo do Módulo 1, com o objetivo de aplicar conhecimentos de **SQL, Python e Análise Exploratória de Dados (EDA)** utilizando uma base de dados de Recursos Humanos (HR).

O projeto foi dividido em duas etapas principais:

1. **Extração dos dados:** realização de consultas SQL na base HR disponibilizada no FreeSQL, utilizando `SELECT`, `LEFT JOIN` e `WHERE` para obter informações específicas das tabelas.
2. **Análise dos dados:** exportação dos resultados das consultas para arquivos `.csv` e posterior realização da Análise Exploratória de Dados utilizando **Python, Pandas e Jupyter Notebook no VS Code**.

Dessa forma, os arquivos CSV utilizados na análise representam os resultados obtidos a partir das consultas realizadas no banco de dados.

---

## 🎯 Objetivos

- Consultar e extrair dados da base HR utilizando SQL.
- Relacionar informações de diferentes tabelas utilizando `LEFT JOIN`.
- Aplicar filtros utilizando `WHERE`.
- Exportar os resultados das consultas para arquivos CSV.
- Realizar uma Análise Exploratória de Dados (EDA) utilizando Python.
- Identificar valores ausentes e registros duplicados.
- Explorar informações relacionadas aos colaboradores, departamentos, países e salários.
- Criar visualizações gráficas para facilitar a interpretação dos dados.
- Identificar padrões e obter insights a partir dos dados analisados.

---

## 🛠️ Tecnologias e ferramentas utilizadas

| Tecnologia/Ferramenta | Utilização |

| FreeSQL | Banco de dados utilizado para consulta da base HR | SQL | Python | Pandas | Matplotlib | Jupyter Notebook | VS Code | Git | GitHub |

---

# 💻 Como executar o projeto

## Pré-requisitos

Para reproduzir a etapa de análise são necessários:

- Python 3;
- Visual Studio Code;
- extensão Python para VS Code;
- extensão Jupyter para VS Code;
- Jupyter Notebook;
- Pandas;
- Matplotlib;

Para a etapa de consultas, é necessário acesso à base HR disponibilizada no FreeSQL.

---

## 📂 Estrutura do projeto

````text
projeto-avaliativo-analise-de-dados/
│
├── README.md
│
|── query_1.sql
│── query_2.sql
│
│── resultado_query_1.csv
│── resultado_query_2.csv
│
|── analise_rh_query01.ipynb
│── analise_rh_query02.ipynb
│
└── .gitignore

# 🔎 Etapas do projeto

## 1. Consulta e extração dos dados

Inicialmente, foram realizadas consultas SQL utilizando a base de dados HR disponibilizada no FreeSQL.

As consultas foram desenvolvidas com o objetivo de obter informações relevantes para a análise, utilizando recursos como:

- `SELECT`;
- `LEFT JOIN`;
- `WHERE`;
- agrupamentos e ordenações, quando necessários.

Os relacionamentos entre as tabelas permitiram reunir informações provenientes de diferentes conjuntos de dados da base HR.

Após a execução das consultas, os resultados foram exportados para arquivos no formato `.csv`.

## 2. Geração dos arquivos CSV

Os resultados obtidos nas consultas SQL foram armazenados em arquivos CSV.

Esses arquivos passaram a ser a **fonte de dados utilizada na etapa de análise exploratória em Python**.

O fluxo utilizado no projeto foi:

```text
Base HR — FreeSQL
       ↓
Consultas SQL
       ↓
Resultados das consultas
       ↓
Arquivos CSV
       ↓
Jupyter Notebook
       ↓
Pandas
       ↓
Análise Exploratória de Dados
       ↓
Visualizações
       ↓
Insights
````

Essa separação permitiu utilizar o SQL para a etapa de extração e o Python para a exploração e interpretação dos dados.

# 🐍 3. Análise Exploratória de Dados — EDA

A Análise Exploratória de Dados foi realizada utilizando **Python e Jupyter Notebook**, executado no **Visual Studio Code**.

Os arquivos CSV gerados a partir das consultas SQL foram carregados utilizando a biblioteca Pandas.

Durante a EDA foram realizadas análises como:

- visualização inicial dos dados;
- identificação da quantidade de linhas e colunas;
- análise dos tipos de dados;
- identificação de valores ausentes;
- identificação de registros duplicados;
- análise estatística dos dados;
- agrupamentos por diferentes categorias;
- análise de colaboradores por país;
- análise de colaboradores por departamento;
- análise da distribuição dos salários.

A partir dos DataFrames criados, foram realizadas as análises e transformações necessárias para compreender os dados.

---

# 📊 4. Visualização dos dados

Após a exploração dos dados, foram criadas visualizações gráficas utilizando Python.

Entre as visualizações desenvolvidas estão:

- **Gráficos de dispersão**, utilizados para analisar a distribuição dos salários;
- **Gráficos de barras**, utilizados para representar a quantidade de colaboradores por país e departamento.

As visualizações foram desenvolvidas dentro do Jupyter Notebook e utilizadas como apoio à interpretação dos resultados encontrados durante a análise.

---

# 📈 5. Principais resultados e insights

A análise dos arquivos CSV permitiu explorar diferentes características da base de Recursos Humanos.

Entre os pontos analisados estão:

### 👥 Colaboradores

Foi analisada a distribuição dos colaboradores entre diferentes países e departamentos, permitindo identificar onde existe maior concentração de funcionários.
Foi constatado que a maioria dos vendedores da empresa, estão concentrados no reino unido, enquanto a maioria dos colaboradores do shipping se concentra nos Estados Unidos.

### 💰 Salários

A distribuição dos salários foi analisada por meio de medidas estatísticas e visualizações gráficas, permitindo observar a concentração dos valores e possíveis diferenças entre os grupos analisados. Ficou claro que as maiores médias salriais ficam com os setores executivo, contabilidade e relações públicas. E as menores medias ficam com os setores de expedição e compras.

### 🏢 Departamentos

A quantidade de colaboradores foi comparada entre os departamentos, possibilitando identificar as áreas com maior e menor quantidade de funcionários. Os departamentos de expediçao e compras são os que possuem mais colaboradores

### 🌎 Distribuição geográfica

Os dados foram agrupados por país para analisar a distribuição dos colaboradores e identificar diferenças na concentração de funcionários entre as localidades.
Ficando evidente que os Estados Unidos possuem a maior força de trabalho da empresa.

### 🧹 Qualidade dos dados

Durante a EDA também foram verificadas informações relacionadas à qualidade dos dados, incluindo:

- valores ausentes;
- registros duplicados;
- tipos das variáveis;
- consistência das informações utilizadas nas análises.

Foram encontrados problemas no registro de alguns colaboradores, o que deve ser passado para a equipe de rh para atualização desses dados.

## Instalação das bibliotecas

No terminal do VS Code, execute:

```bash
pip install pandas matplotlib jupyter
```

---

## Executando a análise

### 1. Clone o repositório

```bash
git clone https://github.com/geraldoMartins22/projeto-avaliativo-analise-de-dados.git
```

### 2. Acesse a pasta

```bash
cd projeto-avaliativo-analise-de-dados
```

### 3. Abra o projeto no VS Code

```bash
code .
```

### 4. Abra o Jupyter Notebook

Acesse a pasta correspondente ao notebook que você deseja e abra:

```text
analise_rh_query01.ipynb ou analise_rh_query02.ipynb
```

### 5. Verifique os arquivos CSV

Antes de executar o notebook, certifique-se de que os arquivos CSV utilizados pela análise estejam na pasta indicada no código.

### 6. Execute as células

Execute as células do notebook na sequência apresentada para reproduzir as etapas da Análise Exploratória de Dados e as visualizações.

---

# 📁 Arquivos SQL

Os arquivos presentes na pasta `.sql` contêm as consultas utilizadas para extrair os dados da base HR.

As consultas são responsáveis pela etapa de **extração dos dados**, enquanto os arquivos CSV gerados a partir delas são utilizados posteriormente na análise com Python.

---

# 📄 Arquivos CSV

Os arquivos CSV contêm os resultados obtidos a partir das consultas realizadas no banco de dados.

Eles são utilizados como fonte de dados pelo Jupyter Notebook durante a etapa de Análise Exploratória de Dados.

---

# 📓 Jupyter Notebook

Os notebooks de análise reúnem a etapa de análise realizada em Python.

Nele estão presentes:

- carregamento dos arquivos CSV;
- exploração dos DataFrames;
- tratamento dos dados;
- análises estatísticas;
- agrupamentos;
- criação das visualizações;
- interpretação dos resultados.

O notebook foi desenvolvido e executado utilizando o **Jupyter Notebook integrado ao Visual Studio Code**.

---

# 🎥 Vídeo de apresentação

O vídeo de apresentação demonstra o desenvolvimento do projeto, incluindo:

- objetivo da análise;
- consultas SQL;
- geração dos arquivos CSV;
- utilização do Jupyter Notebook;
- Análise Exploratória de Dados;
- visualizações criadas;
- principais resultados e insights.

## 📌 Fluxo geral do projeto

```text
┌──────────────────────┐
│      Base HR         │
│       FreeSQL        │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│     Consultas SQL    │
│ SELECT / JOIN / WHERE│
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│      Arquivos CSV    │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│    Jupyter Notebook  │
│       no VS Code     │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│      Pandas / EDA    │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│      Gráficos        │
│ Histograma / Boxplot │
│     / Barras         │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│       Insights       │
└──────────────────────┘
```
