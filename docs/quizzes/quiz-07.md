# Quiz 07 - Introdução

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. Qual símbolo usamos para criar um grupo de captura?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`[]`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`{}`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `()`">`()`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`<>`
    > Resposta Correta: Parênteses são usados para agrupar e capturar.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. Qual a principal diferença entre `[abc]` e `(abc)`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Não há diferença</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `[abc]` busca uma letra; `(abc)` busca a sequência exata "abc"">`[abc]` busca uma letra; `(abc)` busca a sequência exata "abc"</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">O primeiro é mais rápido</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">O segundo é apenas para números
    > Resposta Correta: Colchetes são conjuntos (OU); Parênteses são grupos (SEQUÊNCIA).</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. Como nos referimos ao primeiro grupo de captura dentro da própria expressão?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`$1`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`#1`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `\1`">`\1`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">group(1)
    > Resposta Correta: Usamos a barra invertida seguida do número do grupo (Backreference).</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. O que acontece se aplicarmos um quantificador a um grupo, como `(ha){3}`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Ele busca "ha" e depois o número 3</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Ele busca a sequência "hahaha"">Ele busca a sequência "hahaha"</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Ele busca "ha" no máximo 3 vezes</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Dá erro de sintaxe
    > Resposta Correta: O quantificador repete todo o conteúdo do grupo.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. Qual grupo representa o "Match completo" (todo o texto encontrado)?</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Grupo 0">Grupo 0</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Grupo 1</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Grupo Final</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">O Regex não numera o match completo
    > Resposta Correta: O Grupo 0 sempre contém o resultado total da expressão.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. Quantos grupos de captura existem no padrão `(\d+)-(\w+)-(\s+)`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">1</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">2</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! 3">3</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">6
    > Resposta Correta: Cada par de parênteses cria um grupo novo.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. Em um motor de substituição (como VS Code ou sed), como costumamos chamar o conteúdo do Grupo 1?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`\1` ou `$1`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`Group1`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`%1`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`{1}`
    > Resposta Correta: Geralmente `$1` ou `\1` dependendo da linguagem.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. Para que serve o grupo de "não-captura" `(?:...)`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Para esconder a senha</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Para agrupar sem salvar o resultado na memória (economiza performance)">Para agrupar sem salvar o resultado na memória (economiza performance)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Para comentar o código</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Para ignorar maiúsculas
    > Resposta Correta: Útil quando você quer apenas agrupar, mas não precisa extrair o dado depois.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. O padrão `(\w)\1` encontrará qual destes textos?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">ab</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! aa">aa</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">a1</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">a
    > Resposta Correta: Ele encontrará qualquer caractere seguido dele mesmo (repetição).</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. Como a numeração de grupos é decidida em grupos aninhados como `((A)B)`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Pela importância</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Pela ordem de abertura dos parênteses (Grupo 1 é o externo, Grupo 2 é o interno)">Pela ordem de abertura dos parênteses (Grupo 1 é o externo, Grupo 2 é o interno)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Aleatoriamente</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">De dentro para fora
    > Resposta Correta: O primeiro `(` que abre define o Grupo 1.</div>
  <div class="quiz-feedback"></div>
</div>

