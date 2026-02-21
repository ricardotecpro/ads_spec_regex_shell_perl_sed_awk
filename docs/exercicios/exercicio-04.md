# Exercícios: Aula 04 – Conjuntos de Caracteres 📦

Praticando com intervalos, colchetes e negação.

---

## 🟢 Nível Básico

### 1. Seleção de Vogais
Texto: `As nuvens se movem rapidamente pelo céu azul.`

- **Tarefa**: Crie um padrão que localize todas as vogais (maiúsculas e minúsculas) usando um único conjunto.

### 2. Intervalos Numéricos
Texto: `O preço subiu de 250 para 380 em apenas 5 dias.`

- **Tarefa**: Use o intervalo `[0-9]` para destacar todos os números. Existe diferença se você usar `\d`?

---

## 🟡 Nível Intermediário

### 3. Letras e a Negação
Texto: `ID: AB-1234 | Status: OK`

- **Tarefa**: Use a negação `[^a-zA-Z]` para encontrar tudo o que NÃO é uma letra. 
- **Reflexão**: O que o Regex encontrou? (Espaços, números e símbolos).

### 4. Intervalos Customizados
Texto: `A nota foi A+, a outra foi C e a última foi F-.`

- **Tarefa**: Crie um conjunto que localize apenas as notas de 'A' até 'C'. Ignore 'F'.

---

## 🔴 Nível Desafio

### 5. Filtrando Senhas Simples
Imagine que uma senha deve ter 4 caracteres, onde todos são obrigatoriamente letras minúsculas entre 'a' e 'f', ou números entre '1' e '5'.

- **Tarefa**: Crie o padrão Regex para validar essa regra (dica: repita o conjunto 4 vezes ou tente adivinhar como simplificar).
- **Teste com**: `abcd`, `1234`, `af15`, `gh78` (estes dois últimos devem falhar).