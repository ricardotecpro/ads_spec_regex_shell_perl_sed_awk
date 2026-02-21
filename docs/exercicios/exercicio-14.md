# Exercícios: Aula 14 – Limpeza e Transformação 🧼

Praticando a modificação e o tratamento de strings.

---

## 🟢 Nível Básico

### 1. Limpeza de Espaços
Texto: `   Olá Mundo!    `

- **Tarefa**: Crie um Regex que remova todos os espaços em branco do início e do fim dessa string.

### 2. Substituição Simples
Texto: `O custo é de 100 reais e o frete 20 reais.`

- **Tarefa**: Troque todas as ocorrências de "reais" pelo símbolo "R$".

---

## 🟡 Nível Intermediário

### 3. Criando Slugs de URL
Texto: `Como aprender Regex rápido`

- **Tarefa**: Transforme esse título em um slug de URL amigável: `como-aprender-regex-rapido`.
- **Passos**: 
    1. Transforme espaços em hífens `-`.
    2. Converta tudo para minúsculo (via código JS ou Python).

### 4. Mudando Formato de Telefone
Texto: `1199998888` (Apenas números)

- **Tarefa**: Use grupos de captura para transformar esse texto no formato `(11) 9999-8888`.
- **Substituição**: `($1) $2-$3`.

---

## 🔴 Nível Desafio

### 5. Limpador de Tags XML/HTML
Texto: `<div>Conteúdo <b>Importante</b></div>`

- **Tarefa**: Crie um Regex que remova todas as tags HTML e retorne apenas o texto puro: `Conteúdo Importante`.
- **Desafio**: Garanta que o Regex funcione com qualquer tag (div, b, p, etc).