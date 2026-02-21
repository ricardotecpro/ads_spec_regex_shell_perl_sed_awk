# Exercícios: Aula 03 – Metacaracteres Fundamentais 🔣

Dominando o ponto, classes de caracteres e o escape.

---

## 🟢 Nível Básico

### 1. Uso do Coringa
Texto: `pato, pelo, polo, pulo, p8lo`.

- **Tarefa**: Crie um padrão usando o ponto `.` que localize todas essas palavras de 4 letras que começam com 'p' e terminam com 'lo' ou 'to'.
- **Padrão sugerido**: `p.lo` (Veja quais ele ignora).

### 2. Localizando Números
Texto: `O código do produto é 948 e o lote é o 002.`

- **Tarefa**: Use o metacaractere `\d` para encontrar todos os dígitos isoladamente. Quantos matches você encontrou no total?

---

## 🟡 Nível Intermediário

### 3. O Desafio do Espaço
Texto: `Nome: Ricardo Pires | Idade: 30`

- **Tarefa**: Crie um padrão que utilize `\s` para encontrar os espaços entre o nome e o sobrenome, e entre a idade e o número.

### 4. Alfanuméricos e Underline
Texto: `user_01, admin-02, guest_v3`.

- **Tarefa**: Use `\w` para encontrar os caracteres. 
- **Questão**: O `\w` deu match no hífen `-` do `admin-02`? Por que?

---

## 🔴 Nível Desafio

### 5. Endereços de IP e o Escape
Texto: `O servidor DNS é 8.8.8.8 e o gateway é 192.168.1.1`.

- **Tarefa**: Crie um Regex que localize exatamente o IP `8.8.8.8`. 
- **Importante**: Se você usar `8.8.8.8` sem o escape, seu padrão também encontraria `8A8B8C8`? Prove isso no Regex101.
- **Dica**: Use `\` antes de cada ponto.