# Exercícios: Aula 07 – Agrupamentos e Captura 🎯

Trabalhando com parênteses, grupos e referências.

---

## 🟢 Nível Básico

### 1. Agrupando Repetições
Texto: `ha ha ha haaaaa!`

- **Tarefa**: Use parênteses para agrupar o padrão `(ha )` e adicione um quantificador para encontrar as repetições de "ha ".

### 2. Captura Simples
Texto: `Nome: Ricardo | Sobrenome: Pires`

- **Tarefa**: Crie dois grupos de captura: um para o nome e outro para o sobrenome. Verifique no painel do Regex101 se os grupos 1 e 2 contêm os valores corretos.

---

## 🟡 Nível Intermediário

### 3. Extraindo Dados de Logs
Texto: `[2024-10-21] INFO: Servidor iniciado.`

- **Tarefa**: Crie um padrão que capture apenas a data dentro dos colchetes em um grupo, e o nível do log (INFO) em outro grupo.

### 4. Referências Internas (Backreferences)
Texto: `O código secreto é 123-123. O outro é 456-789.`

- **Tarefa**: Crie um Regex que identifique padrões onde o número antes do hífen seja igual ao número depois do hífen. 
- **Dica**: Use `(\d{3})-\1`.

---

## 🔴 Nível Desafio

### 5. Reorganizando Datas
Texto: `2024-12-25` (Formato AAAA-MM-DD)

- **Tarefa**: Crie três grupos de captura para Ano, Mês e Dia. 
- **Desafio**: Imagine que você quer transformar isso para o formato brasileiro `DD/MM/AAAA`. Como você faria a substituição usando `$1`, `$2` e `$3`? (Apenas descreva ou teste na aba "Substitution" do Regex101).