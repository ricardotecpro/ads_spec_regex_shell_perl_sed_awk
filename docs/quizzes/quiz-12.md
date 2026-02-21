# Quiz 12 - Introdução

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. Qual a função das âncoras `^` e `$` na validação de dados?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Mudar a cor do texto</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Garantir que o padrão corresponda a toda a entrada, sem extras">Garantir que o padrão corresponda a toda a entrada, sem extras</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Permitir que o usuário digite qualquer coisa</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Deixar a busca mais rápida
    > Resposta Correta: Âncoras evitam que o Regex aceite apenas uma parte do texto (ex: validar "123" em "abc123xyz").</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. Um Regex básico para CEP no formato `00000-000` é:</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`\d{8}`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`[0-9]-[0-9]`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `\d{5}-\d{3}`">`\d{5}-\d{3}`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`\w{5}-\w{3}`
    > Resposta Correta: `\d` representa dígitos e `{n}` a quantidade.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. Como tornamos um caractere opcional em uma validação (ex: o ponto no CPF)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Usando `*`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Usando `+`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Usando `?`">Usando `?`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Usando `!`
    > Resposta Correta: O ponto de interrogação `?` significa "zero ou uma vez".</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. Por que validar e-mail com Regex é considerado difícil?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Porque e-mails não aceitam números</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Porque existem muitas regras e excessões na especificação oficial de e-mails">Porque existem muitas regras e excessões na especificação oficial de e-mails</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Porque o símbolo `@` é um metacaractere</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Porque e-mails são criptografados
    > Resposta Correta: A especificação é vasta e complexa, exigindo padrões muito longos para cobertura total.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. O padrão `^\d{3}\.\d{3}\.\d{3}-\d{2}$` valida qual documento?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Título de Eleitor</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! CPF (com pontos e traço)">CPF (com pontos e traço)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">RG</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">CNH
    > Resposta Correta: É a máscara clássica do CPF brasileiro.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. No padrão de telefone `^\(\d{2}\)\s\d{4,5}-\d{4}$`, o que o `\(` faz?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Abre um grupo de captura</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Busca o caractere literal de parênteses (escape)">Busca o caractere literal de parênteses (escape)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">É um erro de digitação</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Inicia um comentário
    > Resposta Correta: Para buscar parênteses reais, precisamos escapar com `\`.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. O padrão `^[0-9]+$` é igual a qual destes?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`^\w+$`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `^\d+$`">`^\d+$`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`^[a-z]+$`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`^.*$`
    > Resposta Correta: `\d` é um atalho para `[0-9]`.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. Para validar uma senha que NÃO pode conter espaços, qual atalho de negação usaríamos?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`\d`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`\w`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `\S` (S maiúsculo)">`\S` (S maiúsculo)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`\D`
    > Resposta Correta: `\S` significa "qualquer coisa que NÃO seja um espaço".</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. O padrão `^([01]\d|2[0-3]):[0-5]\d$` serve para validar:</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Datas</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Horário (formato 24h)">Horário (formato 24h)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Coordenadas GPS</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Versões de software
    > Resposta Correta: Valida horas de 00 a 23 e minutos de 00 a 59.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">59. 10. Regex pode validar se uma data é "real" (ex: recusar 31 de abril)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sim, Regex resolve qualquer lógica</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Não, Regex valida o formato; a lógica do calendário deve ser feita na programação">Não, Regex valida o formato; a lógica do calendário deve ser feita na programação</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sim, mas apenas para anos bissextos</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas se usar a flag global
    > Resposta Correta: Regex é limitado à sintaxe, não conhece regras complexas de calendário.</div>
  <div class="quiz-feedback"></div>
</div>

