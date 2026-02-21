# Exercícios: Aula 06 – Âncoras ⚓

Fixando a posição da busca com início e fim de linha.

---

## 🟢 Nível Básico

### 1. Início de Frase
Texto: `Erro: Falha na conexão. Sistema em Erro.`

- **Tarefa**: Crie um padrão que localize a palavra "Erro" apenas se ela estiver no início da frase.

### 2. Extensões de Arquivos
Texto: `indice.html, estilo.css, script.js, backup.html.old`

- **Tarefa**: Use o `$` para encontrar apenas os arquivos que terminam exatamente com `.html`. 
- **Desafio**: O seu padrão pegou o `backup.html.old`? (Não deveria!).

---

## 🟡 Nível Intermediário

### 3. Validação de Linha Exclusiva
Texto:
```text
12345
abcde
123
123456
```

- **Tarefa**: Crie um Regex que aceite apenas linhas que contenham **exatamente** 5 dígitos (nem mais, nem menos). Use `^` e `$`.

### 4. Começa e Termina
Texto: `A01, B02, C03, A04X`

- **Tarefa**: Localize códigos que começam com 'A' e terminam com um número. 
- **Dica**: Use `^A\d+$` (em testes de linha única no Regex101).

---

## 🔴 Nível Desafio

### 5. O Modo Multiline
Texto:
```text
http://site.com
https://google.com
ftp://servidor.net
```

- **Tarefa**: No Regex101, ative a flag `m` (multiline). Crie um padrão que localize apenas as linhas que começam com `https`.
- **Reflexão**: O que muda se você desativar a flag `m`?