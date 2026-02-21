# Aula 12 – Validação de Dados Reais ✅

Nesta aula, vamos colocar em prática tudo o que aprendemos para construir validadores de dados comuns no dia a dia do desenvolvimento.

---

## 📧 Validação de E-mail

Validar e-mail com Regex é um dos temas mais debatidos, pois existem formatos muito complexos. Vamos focar em uma versão robusta e prática:

- **Padrão**: `^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$`
- **Explicação**:
    - `^...$`: Garante que o texto inteiro é o e-mail.
    - `[a-zA-Z0-9._%+-]+`: Usuário (letras, números e alguns símbolos).
    - `@`: O símbolo obrigatório.
    - `[a-zA-Z0-9.-]+`: Domínio.
    - `\.[a-zA-Z]{2,}`: Extensão (ex: .com, .org, .com.br).

---

## 🆔 Validação de CPF (Formato)

Lembrando que o Regex valida apenas o **formato** (máscara), não a lógica do dígito verificador.

- **Formato**: `000.000.000-00`
- **Padrão**: `^\d{3}\.\d{3}\.\d{3}-\d{2}$`
- **Com pontos opcionais**: `^\d{3}\.?\d{3}\.?\d{3}-?\d{2}$`

---

## 📱 Validação de Telefone (Brasil)

- **Formato**: `(11) 99999-8888`
- **Padrão**: `^\(\d{2}\)\s\d{4,5}-\d{4}$`

---

## 📊 Tabela de Padrões Reais

| Dado | Regex Sugerido |
| :--- | :--- |
| **Data (DD/MM/AAAA)** | `^\d{2}/\d{2}/\d{4}$` |
| **CEP** | `^\d{5}-\d{3}$` |
| **Hora (24h)** | `^([01]\d|2[0-3]):[0-5]\d$` |

---

## 💻 Exemplo em TermynalJS (Validação Única)

<div class="termy">
$ # Validando um CPF via terminal
$ echo "123.456.789-00" | grep -P "^\d{3}\.\d{3}\.\d{3}-\d{2}$"
$ 123.456.789-00
$
$ # Testando um CPF inválido
$ echo "123-456" | grep -P "^\d{3}\.\d{3}\.\d{3}-\d{2}$"
$ # (Nenhum resultado retornado)
</div>

---

## 📝 Exercícios de Fixação

1.  **Básico**: Crie um Regex para validar um CEP no formato `00000-000`.
2.  **Básico**: Melhore o validador de CPF para aceitar tanto números com pontos quanto apenas números (`12345678900`).
3.  **Intermediário**: Crie um validador de URL simples que comece com `https://` e termine com `.com`.
4.  **Intermediário**: Valide um horário no formato `HH:MM`.
5.  **Desafio**: No Regex101, crie um padrão para "Senhas Fortes" que exija: Mínimo 8 caracteres, pelo menos uma letra e pelo menos um número. (Use o que aprendeu, não precisa ser uma única expressão se for difícil demais agora!).

---

## 🚀 Mini-Projeto: Validador de Senhas

**Objetivo**: Verificar se uma senha atende aos requisitos mínimos de segurança.

1.  Regra: A senha deve ter entre 8 e 20 caracteres e conter ao menos um caractere especial (`!@#$%*`).
2.  Regex sugerido: `^[\w!@#$%*]{8,20}$` (Note: este aceita, mas não obriga o especial, para obrigar precisaríamos de *lookaheads*, que é avançado. Por enquanto, valide se ela contém apenas os permitidos e o tamanho).
3.  Teste com: `senha123` (✅), `123` (❌), `senha_muito_longa_que_passa_do_limite` (❌).