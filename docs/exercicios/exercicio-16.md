# Exercícios: Aula 16 – Revisão Geral e Desafios 🏁

Parabéns por chegar ao fim! Estes exercícios revisam os tópicos mais complexos do curso.

---

## 🟢 Nível Básico

### 1. Busca Localizada
- **Tarefa**: Crie um Regex que encontre a palavra "Regex" apenas se ela estiver no início da frase.
- **Teste com**: "Regex é legal" (✅) e "O curso de Regex" (❌).

### 2. Formato de Versão
- **Tarefa**: Valide uma versão de software no formato `v1.2.3`.
- **Dica**: Use `v\d\.\d\.\d`.

---

## 🟡 Nível Intermediário

### 3. Extração de Conteúdo de Tags
Texto: `<h1 id="titulo">Bem-vindo ao Curso</h1>`

- **Tarefa**: Use um grupo de captura para extrair apenas o texto "Bem-vindo ao Curso".
- **Desafio**: Tente extrair também o valor do ID (titulo) em outro grupo.

### 4. Limpeza de Logins de Usuários
Texto: `usuario_01, usuario_02, USER_03, admin`

- **Tarefa**: Use Regex para extrair apenas os usuários que terminam com `_01`, `_02` ou `_03`.

---

## 🔴 Nível Desafio

### 5. Validador de Senha Completo
- **Tarefa**: Crie um script (JS ou Python) que valide se uma senha:
  1. Tem no mínimo 8 caracteres.
  2. Tem pelo menos uma Letra Maiúscula.
  3. Tem pelo menos uma Letra Minúscula.
  4. Tem pelo menos um Número.
  5. Tem pelo menos um Caractere Especial (`!@#$%*`).
- **Dica**: No nível básico, você pode usar 5 Regex separados para validar cada regra!