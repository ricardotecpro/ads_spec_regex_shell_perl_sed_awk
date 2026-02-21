# Exercícios: Aula 01 – Introdução ao Regex 📝

Pratique os conceitos fundamentais de busca e identificação de padrões.

---

## 🟢 Nível Básico

### 1. Busca Literal Direta
No [Regex101](https://regex101.com/), utilize o texto abaixo:
`O aprendizado de Expressões Regulares é um diferencial para o programador moderno.`

- **Tarefa**: Crie um padrão que localize exatamente a palavra "programador".
- **Desafio Extra**: Quantos matches ocorrem se você buscar apenas por "er"?

### 2. Identificação de Plataformas
Cite 3 ferramentas ou linguagens de programação que você utiliza no dia a dia que possuem suporte nativo para Regex. Como você acha que o Regex poderia ajudar no uso dessas ferramentas?

---

## 🟡 Nível Intermediário

### 3. Case Sensitivity na Prática
Utilize o texto: `Regex, regex, REGEX, ReGeX`.

- **Tarefa**: Crie um padrão literal `regex` (minúsculo).
- **Ação**: Ative e desative a flag `i` (ignore case) no seu testador. Explique o que acontece com o número de matches em cada estado.

### 4. Localizando Números Simples
No texto: `Em 1970 surgiram as bases do Regex, e em 2024 ele continua essencial.`

- **Tarefa**: Tente encontrar o número "2024" usando apenas caracteres literais. O que acontece se você buscar por "20 24"?

---

## 🔴 Nível Desafio

### 5. O Primeiro Match Contextual
Imagine que você tem um arquivo de log com milhares de linhas como esta:
`2024-10-21 14:30:05 - ERROR: Database connection failed.`

- **Tarefa**: Crie um padrão que localize apenas a palavra "ERROR". 
- **Reflexão**: Se o log tivesse a palavra "error" (minúscula), seu padrão funcionaria? Como garantir que ele pegue ambos sem usar flags? (Pense em como os conjuntos `[]` poderiam ajudar, mesmo sem tê-los estudado ainda).