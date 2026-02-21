# Exercícios: Aula 11 – Regex com Python 🐍

Utilizando a biblioteca `re` para manipulação de dados.

---

## 🟢 Nível Básico

### 1. Busca Simples
- **Tarefa**: Escreva um código Python que use `re.search()` para verificar se a string `"Sucesso!"` termina com um ponto de exclamação.

### 2. Listagem de Números
- **Tarefa**: Dada a string `"Código: 123, ID: 456, Ref: 789"`, use `re.findall()` para obter uma lista com apenas os números.

---

## 🟡 Nível Intermediário

### 3. Limpeza de Logs
- **Tarefa**: Use `re.sub()` para remover a data (formato `YYYY-MM-DD`) de uma linha de log: `"2024-10-21 - Erro no sistema"`. O resultado deve ser apenas `"- Erro no sistema"`.

### 4. Grupos de Match
- **Tarefa**: Use `re.search()` com parênteses para capturar separadamente o DDD e o número de um telefone: `"(11) 98888-7777"`. Imprima cada grupo separadamente.

---

## 🔴 Nível Desafio

### 5. Analisador de Caminhos (Paths)
- **Tarefa**: Crie um script que receba um caminho de arquivo como `"/home/usuario/documentos/foto.png"` e use Regex para extrair apenas o nome do arquivo (`foto.png`) e apenas a extensão (`png`).
- **Dica**: Use âncoras de fim de linha `$` e classes de caracteres negadas.