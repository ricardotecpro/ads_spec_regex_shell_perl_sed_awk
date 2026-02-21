# Exercícios: Aula 15 – Desempenho e Boas Práticas ⚡

Refatorando expressões para torná-las mais eficientes e seguras.

---

## 🟢 Nível Básico

### 1. Otimizando Alternância
Padrão Original: `(segunda|terça|quarta|quinta|sexta)`

- **Tarefa**: Se você não precisar extrair o dia da semana depois, apenas verificar se existe, como você transformaria esse grupo para economizar memória?

### 2. Substituindo o Coringa
Padrão Original: `.*` (para encontrar um número de 5 dígitos)

- **Tarefa**: Reescreva esse padrão para ser mais específico e performático.

---

## 🟡 Nível Intermediário

### 3. Proteção contra Ataques (ReDoS)
Padrão Original: `(a+)+c`

- **Tarefa**: Analise por que esse padrão é perigoso em textos que contêm muitos 'a's mas não terminam em 'c'. Como você o recreveria de forma simples para pegar uma sequência de letras 'a' seguida de 'c'?

### 4. Uso de Âncoras para Velocidade
- **Tarefa**: Explique por que o padrão `^\d{5}$` é processado mais rápido por um motor de busca do que `\d{5}` em uma string que começa com letras.

---

## 🔴 Nível Desafio

### 5. Auditoria de Validador
Imagine o seguinte Regex para validar um nome de pessoa: `^[a-zA-Z\s]*$`

- **Questões**:
    1. O que acontece se o usuário enviar uma string vazia? (O `*` permite isso).
    2. Como você alteraria para exigir ao menos 2 letras?
    3. Como você limitaria o tamanho máximo para 50 caracteres para evitar processamento abusivo?