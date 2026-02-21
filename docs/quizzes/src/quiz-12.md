# Quiz 12 - Validação de Dados Reais ✅

1. Qual a função das âncoras `^` e `$` na validação de dados?
    - [ ] Mudar a cor do texto
    - [x] Garantir que o padrão corresponda a toda a entrada, sem extras
    - [ ] Permitir que o usuário digite qualquer coisa
    - [ ] Deixar a busca mais rápida
    > Resposta Correta: Âncoras evitam que o Regex aceite apenas uma parte do texto (ex: validar "123" em "abc123xyz").

2. Um Regex básico para CEP no formato `00000-000` é:
    - [ ] `\d{8}`
    - [ ] `[0-9]-[0-9]`
    - [x] `\d{5}-\d{3}`
    - [ ] `\w{5}-\w{3}`
    > Resposta Correta: `\d` representa dígitos e `{n}` a quantidade.

3. Como tornamos um caractere opcional em uma validação (ex: o ponto no CPF)?
    - [ ] Usando `*`
    - [ ] Usando `+`
    - [x] Usando `?`
    - [ ] Usando `!`
    > Resposta Correta: O ponto de interrogação `?` significa "zero ou uma vez".

4. Por que validar e-mail com Regex é considerado difícil?
    - [ ] Porque e-mails não aceitam números
    - [x] Porque existem muitas regras e excessões na especificação oficial de e-mails
    - [ ] Porque o símbolo `@` é um metacaractere
    - [ ] Porque e-mails são criptografados
    > Resposta Correta: A especificação é vasta e complexa, exigindo padrões muito longos para cobertura total.

5. O padrão `^\d{3}\.\d{3}\.\d{3}-\d{2}$` valida qual documento?
    - [ ] Título de Eleitor
    - [x] CPF (com pontos e traço)
    - [ ] RG
    - [ ] CNH
    > Resposta Correta: É a máscara clássica do CPF brasileiro.

6. No padrão de telefone `^\(\d{2}\)\s\d{4,5}-\d{4}$`, o que o `\(` faz?
    - [ ] Abre um grupo de captura
    - [x] Busca o caractere literal de parênteses (escape)
    - [ ] É um erro de digitação
    - [ ] Inicia um comentário
    > Resposta Correta: Para buscar parênteses reais, precisamos escapar com `\`.

7. O padrão `^[0-9]+$` é igual a qual destes?
    - [ ] `^\w+$`
    - [x] `^\d+$`
    - [ ] `^[a-z]+$`
    - [ ] `^.*$`
    > Resposta Correta: `\d` é um atalho para `[0-9]`.

8. Para validar uma senha que NÃO pode conter espaços, qual atalho de negação usaríamos?
    - [ ] `\d`
    - [ ] `\w`
    - [x] `\S` (S maiúsculo)
    - [ ] `\D`
    > Resposta Correta: `\S` significa "qualquer coisa que NÃO seja um espaço".

9. O padrão `^([01]\d|2[0-3]):[0-5]\d$` serve para validar:
    - [ ] Datas
    - [x] Horário (formato 24h)
    - [ ] Coordenadas GPS
    - [ ] Versões de software
    > Resposta Correta: Valida horas de 00 a 23 e minutos de 00 a 59.

10. Regex pode validar se uma data é "real" (ex: recusar 31 de abril)?
    - [ ] Sim, Regex resolve qualquer lógica
    - [x] Não, Regex valida o formato; a lógica do calendário deve ser feita na programação
    - [ ] Sim, mas apenas para anos bissextos
    - [ ] Apenas se usar a flag global
    > Resposta Correta: Regex é limitado à sintaxe, não conhece regras complexas de calendário.