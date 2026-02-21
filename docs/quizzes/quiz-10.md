# Quiz 10 - Introdução

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. Qual a forma mais comum de declarar um Regex literal em JavaScript?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`new RegExp("padrao")`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `/padrao/`">`/padrao/`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`regex("padrao")`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`"padrao".toRegex()`
    > Resposta Correta: A sintaxe entre barras `/.../` é a mais utilizada.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. Qual método do objeto Regex retorna apenas `true` ou `false`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`.match()`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`.search()`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `.test()`">`.test()`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`.exec()`
    > Resposta Correta: `.test()` é ideal para validações booleanas.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. Onde o método `.match()` deve ser chamado?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">No objeto Regex (`regex.match(texto)`)</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Na própria String (`texto.match(regex)`)">Na própria String (`texto.match(regex)`)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Globalmente</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">No console
    > Resposta Correta: `.match()` é um método do protótipo de String.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. O que o método `.match()` retorna quando não encontra nada?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Um array vazio `[]`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`false`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `null`">`null`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`undefined`
    > Resposta Correta: No JavaScript, se não houver match, o retorno é `null`.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. Qual método usamos para substituir textos usando Regex no JavaScript?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`.change()`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `.replace()`">`.replace()`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`.substitute()`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`.map()`
    > Resposta Correta: `.replace()` aceita tanto strings simples quanto Regex.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. O que a flag `g` faz no método `.replace()`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Nada, ela é ignorada</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Substitui apenas a primeira ocorrência</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Garante que TODAS as ocorrências sejam substituídas">Garante que TODAS as ocorrências sejam substituídas</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Torna a substituição invisível
    > Resposta Correta: Sem o `g`, o JavaScript substitui apenas a primeira por padrão.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. Como passamos flags ao criar um Regex com `new RegExp()`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`/padrao/gi`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `new RegExp("padrao", "gi")` (como segundo argumento)">`new RegExp("padrao", "gi")` (como segundo argumento)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`new RegExp("padrao/gi")`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Não é possível passar flags
    > Resposta Correta: O segundo parâmetro da função construtora aceita as flags.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. O padrão `/\d+/` dará match em qual valor do objeto `test("Aula 10")`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">"Aula"</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">" " (espaço)</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! true">true</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">10
    > Resposta Correta: O método `.test()` retorna booleano, e como há números, retornará `true`.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. O método `.replaceAll()` (adicionado recentemente no JS) exige que o Regex tenha qual flag?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Flag `i`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Flag `g`">Flag `g`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Flag `m`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Não exige nenhuma flag
    > Resposta Correta: O `replaceAll` com Regex lança erro se a flag global não estiver presente.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. Qual a principal vantagem de usar Regex literais em vez do construtor `new RegExp()`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">É mais lento</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! É mais legível e processado mais rápido pelo motor JS (estático)">É mais legível e processado mais rápido pelo motor JS (estático)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Aceita variáveis dentro dele</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Não precisa de barras
    > Resposta Correta: Literais são analisados no momento do carregamento do script.</div>
  <div class="quiz-feedback"></div>
</div>

