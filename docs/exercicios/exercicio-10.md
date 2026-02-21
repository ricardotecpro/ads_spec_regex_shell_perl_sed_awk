# Exercícios: Aula 10 – Regex com JavaScript 📜

Aplicando Regex no ecossistema Web.

---

## 🟢 Nível Básico

### 1. Validação de Booleano
- **Tarefa**: Crie um script em JavaScript que use o método `.test()` para validar se uma string contém apenas números.
- **Teste com**: `"12345"` (true) e `"123a45"` (false).

### 2. Busca de Palavras
- **Tarefa**: Dado o texto `"JavaScript é incrível"`, use `.match()` para encontrar a palavra "JavaScript".

---

## 🟡 Nível Intermediário

### 3. Substituição de Padrões
- **Tarefa**: Use o método `.replace()` para mascarar os 4 últimos dígitos de um cartão de crédito: `"4555.2222.1111"`. Transforme em `"4555.2222.****"`.
- **Dica**: Use o quantificador `{4}$`.

### 4. Extração Global
- **Tarefa**: Extraia todas as palavras que começam com a letra "R" da frase: `"Regex é Rápido, Robusto e Real"`. Use a flag `gi`.

---

## 🔴 Nível Desafio

### 5. Validador de Senha
- **Tarefa**: Crie uma função `validarSenha(senha)` que retorne `true` apenas se a senha tiver:
  - No mínimo 8 caracteres.
  - Pelo menos um número.
  - Pelo menos uma letra maiúscula.
- **Dica**: Você pode usar múltiplos `.test()` ou tentar uma expressão regular avançada única.