# Quiz 11 - Introdução

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. Qual biblioteca do Python é usada para trabalhar com Expressões Regulares?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`regex`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `re`">`re`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`math`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`os`
    > Resposta Correta: O módulo `re` é a biblioteca padrão.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. O que significa o prefixo `r` em uma string Regex (ex: `r"\d"`)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Read-only</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Raw String (String Bruta), preservando as barras invertidas">Raw String (String Bruta), preservando as barras invertidas</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Replace mode</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Regex mode
    > Resposta Correta: Evita que o Python interprete escapes como `\n` ou `\t`.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. Qual função encontra a PRIMEIRA ocorrência de um padrão em uma string?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`re.findall()`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `re.search()`">`re.search()`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`re.match()`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`re.sub()`
    > Resposta Correta: `re.search()` varre a string toda em busca da primeira chance.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. Qual a diferença entre `re.match()` e `re.search()` no Python?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Nenhuma</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `match` só procura no INÍCIO da string; `search` procura em QUALQUER lugar">`match` só procura no INÍCIO da string; `search` procura em QUALQUER lugar</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`search` é mais rápido</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`match` retorna uma lista
    > Resposta Correta: `re.match()` é implícitamente ancorado no começo.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. Qual função retorna uma LISTA com todos os matches encontrados?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`re.list()`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`re.search_all()`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `re.findall()`">`re.findall()`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`re.extract()`
    > Resposta Correta: `findall()` é ideal para extrair coleções de dados.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. Como substituímos um padrão por outro texto usando o módulo `re`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`re.replace()`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`re.change()`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `re.sub()`">`re.sub()`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`re.swap()`
    > Resposta Correta: `sub` vem de "substitute".</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. O que a função `re.findall()` retorna se não encontrar nenhuma ocorrência?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`None`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Uma lista vazia `[]`">Uma lista vazia `[]`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Um erro de sistema</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`False`
    > Resposta Correta: Retorna uma lista vazia, facilitando loops `for`.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. Para acessar o conteúdo capturado por um grupo em `re.search()`, usamos:</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`.content()`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `.group()` ou `.groups()`">`.group()` ou `.groups()`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`.text()`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`[0]`
    > Resposta Correta: O objeto Match possui o método `.group()`.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. No Python, as flags (como IgnoreCase) são passadas como:</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`/padrao/i`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Um argumento opcional: `re.search(p, s, flags=re.IGNORECASE)`">Um argumento opcional: `re.search(p, s, flags=re.IGNORECASE)`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Não existem flags no Python</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">No início do padrão: `(i)padrao`
    > Resposta Correta: São passadas através do argumento `flags` usando constantes do módulo `re`.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. O padrão `re.split(r"\s+", texto)` resultará em:</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Uma string sem espaços</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Uma lista de palavras separadas pelos espaços">Uma lista de palavras separadas pelos espaços</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Um erro de tipo</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas o primeiro espaço
    > Resposta Correta: `split` divide a string baseada no padrão Regex.</div>
  <div class="quiz-feedback"></div>
</div>

