# Exercícios: Aula 08 – Alternância 🔀

Praticando o uso do "OU" e a prioridade de padrões.

---

## 🟢 Nível Básico

### 1. Seleção Simples
Texto: `O gato dormiu no tapete, mas o cachorro preferiu o sofá.`

- **Tarefa**: Crie um padrão que localize as palavras "gato" ou "cachorro".

### 2. Opções de Arquivos
Texto: `projeto.html, estilo.css, script.js`

- **Tarefa**: Crie um Regex que identifique se o arquivo tem extensão `.html` ou `.js`.

---

## 🟡 Nível Intermediário

### 3. Alternância com Agrupamento
Texto: `Eu gosto de café. Você gosta de chá?`

- **Tarefa**: Use parênteses para agrupar as opções de bebida: `gosta de (café|chá)`.
- **Reflexão**: O que acontece se você remover os parênteses e deixar `gosta de café|chá`?

### 4. Prioridade de Match
Texto: `super, supercomputador`

- **Tarefa**: Tente dar match em `supercomputador|super` e depois em `super|supercomputador`. Como o Regex se comporta no segundo caso ao encontrar a palavra longa?

---

## 🔴 Nível Desafio

### 5. Validando Respostas curtas
Texto: `Resposta: Sim, Resposta: Não, Resposta: Talvez`

- **Tarefa**: Crie um padrão que capture apenas o que vem depois de "Resposta: " se for as palavras "Sim" ou "Não". Ignore "Talvez".
- **Dica**: Use `Resposta:\s(Sim|Não)`.
- **Extra**: Como você faria para aceitar "S" ou "N" também?