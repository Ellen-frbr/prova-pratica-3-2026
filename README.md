# Prova Prática — Ciência de Dados com Python 🐍📊

**Curso:** Ciência de Dados com Python (40h)
**Ferramentas:** Google Colab · Python 3 · NumPy · Pandas · Matplotlib · Seaborn

---

## 📌 Sobre a prova

Esta é a prova prática do curso. Você deverá resolver **10 questões** em um notebook Jupyter,
aplicando tudo o que aprendeu nas aulas de NumPy, Pandas, Matplotlib e Seaborn —
da importação dos dados até a visualização.

- 📁 **Arquivos da prova:**
  - `prova_pratica_ciencia_de_dados.ipynb` — notebook com as questões (é nele que você responde)
  - `vendas_loja.csv` — base de dados utilizada
- 🎯 **Valor:** 10,0 pontos (1,0 por questão)
- ⏱️ **Duração:** 4 horas

---

## 🚀 Como começar

1. Baixe os dois arquivos deste repositório (`prova_pratica_ciencia_de_dados.ipynb` e `vendas_loja.csv`).
2. Acesse [colab.research.google.com](https://colab.research.google.com) e faça upload do notebook
   (**Arquivo → Fazer upload do notebook**).
3. Faça upload do dataset clicando no ícone de pasta 📁 na barra lateral do Colab e arrastando
   o arquivo `vendas_loja.csv`.
4. Execute a célula de importação das bibliotecas (célula 2 do notebook) e comece a prova!

---

## 📁 Sobre o dataset

O arquivo `vendas_loja.csv` contém os registros de vendas de uma loja de eletrônicos,
com **120+ linhas** e as seguintes colunas:

| Coluna | Descrição |
|---|---|
| `produto` | Nome do produto vendido |
| `categoria` | Categoria do produto (Informática, Áudio, Acessórios, Armazenamento) |
| `preco` | Preço unitário do produto (R$) |
| `quantidade` | Quantidade de unidades vendidas |
| `vendedor` | Nome do vendedor responsável |
| `regiao` | Região da loja (Norte, Sul, Leste, Oeste) |
| `mes` | Mês da venda (Jan a Jun) |

> ⚠️ **Atenção:** o dataset contém **valores ausentes e linhas duplicadas de propósito** —
> você vai precisar tratá-los nas questões 4 e 5. Não tente "corrigir" o CSV manualmente:
> o objetivo é resolver isso com código!

---

## 📝 Questões

| # | Tema | O que fazer |
|---|---|---|
| 1 | Importação e exploração | Importar o CSV e mostrar `head`, `shape` e `info` |
| 2 | Exploração | Rodar `describe()` e interpretar a média de `preco` |
| 3 | NumPy | Transformar `preco` em array e calcular média, máx, mín e `size` |
| 4 | Valores ausentes | Contar ausentes e tratá-los com `fillna` (justificando a escolha) |
| 5 | Duplicados | Detectar com `duplicated()` e remover com `drop_duplicates()` |
| 6 | Coluna calculada | Criar a coluna `total` = `preco` × `quantidade` |
| 7 | Filtro simples | Filtrar vendas com `total` ≥ 500 |
| 8 | Filtro composto | Filtrar região `'Sul'` com `quantidade` > 5 (usar `&`) |
| 9 | Agrupamento | `groupby` por categoria + resumo com `agg` |
| 10 | Visualização | Gráfico de barras (Matplotlib) + boxplot por região (Seaborn) |

O notebook já traz cada questão com seu enunciado detalhado e uma célula de código vazia
para você escrever sua resposta.

---

## ✅ Regras e critérios de avaliação

1. **Resolva com o código.** As questões de filtro, limpeza e agrupamento devem ser feitas
   com os comandos do curso (`fillna`, `drop_duplicates`, `groupby`, etc.) — não vale
   editar o CSV na mão.
2. **O notebook precisa rodar do início ao fim sem erros.** Antes de entregar, use
   **Runtime → Run all** no Colab e confira.
3. As questões que pedem interpretação (2, 4 e 9) só ganham ponto integral **com a frase
   escrita** explicando o resultado.
4. Os gráficos da questão 10 precisam ter **título e eixos nomeados**.

### Rubrica

| Critério | Questões | Pontos |
|---|---|---|
| Importação e exploração | 1 e 2 | 2,0 |
| NumPy | 3 | 1,0 |
| Limpeza de dados (ausentes e duplicados) | 4 e 5 | 2,0 |
| Manipulação com Pandas (coluna e filtros) | 6, 7 e 8 | 3,0 |
| Agrupamento e resumo | 9 | 1,0 |
| Visualização | 10 | 1,0 |
| **Total** | | **10,0** |

---

## 📤 Como entregar

1. No Colab: **Arquivo → Fazer download → Fazer download do .ipynb**
2. Envie o arquivo `prova_pratica_ciencia_de_dados.ipynb` com seu nome no padrão:
   `prova_nome_sobrenome.ipynb` (ex.: `prova_maria_silva.ipynb`)
3. Submeta pelo link/formulário indicado pelo professor.

---

## 💡 Dicas

- Travou em alguma questão? Pule e volte depois — a prova cobre aulas diferentes e é
  comum uma questão ajudar a lembrar o conteúdo de outra.
- Erro de leitura do arquivo? Confira se o `vendas_loja.csv` foi para a pasta raiz do Colab.
- Regra de bolso do curso: **nunca analise o que você ainda não explorou** —
  comece sempre com `head`, `shape`, `info` e `describe`.

**Boa prova! 🚀**
