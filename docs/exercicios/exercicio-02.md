# Exercícios: Aula 02 – Estrutura Básica 🏗️

Aprofundando em buscas literais e sensibilidade de caixa.

---

## 🟢 Nível Básico

### 1. Buscando Marcas e Nomes
Texto: `O iPhone, o iPad e o MacBook são produtos da Apple.`

- **Tarefa**: Localize a palavra `Apple`.
- **Questão**: Se você buscar por `apple`, o match ocorre? Por que?

### 2. Espaços e Símbolos
Texto: `Preço: R$ 50,00 | Desconto: 10%`

- **Tarefa**: Tente dar match exatamente em `R$ 50,00`. 
- **Atenção**: Lembre-se que espaços contam como caracteres!

---

## 🟡 Nível Intermediário

### 3. Palavras Combinadas
Texto: `O curso de Regex é excelente. Eu amo regex!`

- **Tarefa**: Crie um padrão que encontre as duas ocorrências da palavra "regex", independente de ser maiúscula ou minúscula, utilizando a flag `i`.

### 4. Filtro de Substrings
Texto: `casa, casarão, casado, casulo`.

- **Tarefa**: Busque pela palavra literal `casa`. 
- **Observação**: Quantos matches você obteve? Ele pegou partes de outras palavras ou apenas a palavra isolada? Por que isso acontece no Regex literal?

---

## 🔴 Nível Desafio

### 5. Simulando um Finder
Crie uma lista de 10 nomes de arquivos fictícios (ex: `foto.jpg`, `relatorio.pdf`, `musica.mp3`).

- **Tarefa**: Crie um Regex literal para encontrar todos os arquivos que terminam em `.jpg`.
- **Reflexão**: Como você faria para encontrar arquivos `.JPG` e `.jpg` ao mesmo tempo sem usar flags?