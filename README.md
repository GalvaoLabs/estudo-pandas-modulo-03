# 🐼 Primeiros passos com Pandas

Notebook Jupyter de estudo que apresenta os conceitos básicos da biblioteca [Pandas](https://pandas.pydata.org/), com explicações, exemplos práticos e uma lista de exercícios resolvidos.

## 📚 Conteúdo

### Teoria e exemplos

- **Instalação e importação** do Pandas
- **Series**: estrutura unidimensional com índice
  - Principais métodos: `head()`, `tail()`, `unique()`, `value_counts()`, `mean()`, `sum()`, `max()`/`min()`, `sort_values()`, `isnull()`/`notnull()` e `apply()`
  - Exemplo com uma lista de 100 notas convertida em Series
- **DataFrame**: estrutura bidimensional (linhas e colunas)
  - Principais métodos: `head()`, `info()`, `describe()`, `shape`, `columns`, `dtypes`, `loc[]`, `iloc[]`, `drop()`, `groupby()`, `sort_values()`, `fillna()`, `merge()`, `to_csv()`/`read_csv()`
  - Criação de um DataFrame a partir de um dicionário
  - Seleção de colunas
  - Cálculo de média
  - Filtragem de linhas com condições booleanas
  - Análise da estrutura com `df.info()`

### Exercícios

Os exercícios usam um DataFrame de funcionários com as colunas `nome`, `unidade`, `escala_noturna` e `vendas`.

| # | Exercício                                            | Conceito praticado     |
|---|------------------------------------------------------|------------------------|
| 1 | Importar o Pandas como `pd`                          | Importação             |
| 2 | Transformar um dicionário em DataFrame               | Criação de DataFrame   |
| 3 | Exibir dimensões, colunas e tipos de dados           | `info()`               |
| 4 | Contar funcionários por unidade                      | `value_counts()`       |
| 5 | Contar funcionários por turno (dia ou noite)         | `value_counts()`       |
| 6 | Encontrar as vendas de Henrique Costa                | Filtragem              |
| 7 | Listar quem vendeu menos de R$ 20.000                | Filtragem com condição |
| 8 | (Bônus) Comparar o total de vendas do dia e da noite | Filtragem e `sum()`    |

## ⚙️ Pré-requisitos

- Python 3.8 ou superior
- Pandas
- Jupyter Notebook, JupyterLab ou VS Code com a extensão Jupyter

## 📦 Instalação

1. Clone ou baixe este repositório.
2. (Opcional) Crie e ative um ambiente virtual:

```bash
python -m venv venv
source venv/bin/activate      # Linux/macOS
venv\Scripts\activate         # Windows
```

3. Instale as dependências:

```bash
pip install pandas jupyter
```

## ▶️ Como executar

Abra o notebook com o Jupyter:

```bash
jupyter notebook
```

Depois abra o arquivo `.ipynb` no navegador. Se preferir, abra o arquivo diretamente no VS Code.

## 🗂️ Estrutura do projeto

```
pandas-primeiros-passos/
├── pandas_01.ipynb
└── README.md
```

## 📊 Exemplo de resultado

No exercício bônus, o notebook compara as vendas por turno:

```
Vendas de noite: R$: 189655.03
Vendas de dia: R$: 152742.46
```

## 💡 Dicas de estudo

- Execute as células na ordem, de cima para baixo.
- Teste os métodos que não foram demonstrados nos exemplos, como `describe()`, `sort_values()` e `groupby()`.
- Nas células de exercício, as respostas já estão preenchidas. Para praticar, apague o código e tente resolver sozinho antes de comparar.

## 📄 Licença

Projeto de uso livre para fins de estudo.
