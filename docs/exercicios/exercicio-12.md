# Exercícios: Aula 12 – Validação de Dados Reais ✅

Praticando a validação de formatos comuns do dia a dia.

---

## 🟢 Nível Básico

### 1. CEP Brasileiro
- **Tarefa**: Crie um Regex que valide um CEP no formato `00000-000`.
- **Teste com**: `04101-000` (✅) e `04101000` (❌).

### 2. Formato de Data
- **Tarefa**: Crie um padrão que valide uma data no formato `DD/MM/AAAA`.
- **Dica**: Use `\d{2}/\d{2}/\d{4}`.

---

## 🟡 Nível Intermediário

### 3. Validação de CPF Flexível
- **Tarefa**: Crie um Regex que valide um CPF, aceitando tanto o formato com pontos e traço (`123.456.789-00`) quanto apenas números (`12345678900`).
- **Dica**: Use o ponto de interrogação `?` para tornar os separadores opcionais.

### 4. Horário em 24h
- **Tarefa**: Crie um Regex que valide um horário entre `00:00` e `23:59`.
- **Dica**: O primeiro dígito pode ser `[01]` seguido de qualquer número, OU `2` seguido de `[0-3]`.

---

## 🔴 Nível Desafio

### 5. Validador de E-mail Corporativo
- **Tarefa**: Crie um Regex que valide apenas e-mails que pertençam ao domínio `@empresa.com.br`.
- **Atenção**: Garante que não haja nada antes ou depois do e-mail na linha.
- **Teste com**: `joao@empresa.com.br` (✅), `joao@gmail.com` (❌), `contato@empresa.com.br.suporte` (❌).