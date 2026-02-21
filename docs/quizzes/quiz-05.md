# Quiz 05 - Introdução

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. Qual símbolo representa "zero ou mais ocorrências"?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`+`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`?`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `*`">`*`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`{0}`
    > Resposta Correta: O asterisco `*` permite que o padrão apareça nunca ou muitas vezes.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. Qual a diferença entre `*` e `+`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`*` é para números e `+` para letras</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `+` exige ao menos uma ocorrência; `*` aceita zero">`+` exige ao menos uma ocorrência; `*` aceita zero</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`*` é mais rápido</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Não há diferença
    > Resposta Correta: O sinal de mais `+` significa "um ou mais".</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. O que o quantificador `{3}` faz?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Busca o número 3 no texto</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Faz com que o padrão anterior se repita exatamente 3 vezes">Faz com que o padrão anterior se repita exatamente 3 vezes</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Busca no máximo 3 vezes</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Indica a terceira linha do arquivo
    > Resposta Correta: Define uma quantidade exata de repetições.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. Como escrevemos um padrão que aceite de 2 a 5 dígitos?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`\d{2-5}`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `\d{2,5}`">`\d{2,5}`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`\d(2,5)`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`\d[2-5]`
    > Resposta Correta: A sintaxe correta usa vírgula `{m,n}`.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. O que significa o símbolo `?` quando usado sozinho após um caractere?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Uma pergunta ao motor de busca</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Que o caractere anterior é opcional (zero ou uma vez)">Que o caractere anterior é opcional (zero ou uma vez)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Que o texto é um link</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Que a busca deve parar
    > Resposta Correta: O ponto de interrogação torna o item anterior opcional.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. O que é um quantificador "Guloso" (Greedy)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Um que trava o computador</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Um que tenta capturar o maior trecho de texto possível">Um que tenta capturar o maior trecho de texto possível</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Um que só busca palavras longas</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Um que ignora espaços
    > Resposta Correta: Ele consome o máximo de caracteres que casam com o padrão.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. Como transformamos um quantificador guloso (como `.*`) em "Preguiçoso" (Lazy)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Usando a flag `/L`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Colocando um `+` no final</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Colocando um `?` logo após o quantificador (ex: `.*?`)">Colocando um `?` logo após o quantificador (ex: `.*?`)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Diminuindo o tamanho do texto
    > Resposta Correta: O `?` após outro quantificador muda seu comportamento para o mínimo possível.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. O padrão `[0-9]{2,}` significa:</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Exatamente 2 números</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">No máximo 2 números</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! No mínimo 2 números (sem limite superior)">No mínimo 2 números (sem limite superior)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Números que terminam com vírgula
    > Resposta Correta: Deixando o segundo valor vazio `{2,}`, remove-se o limite máximo.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. Se eu buscar `ba*` no texto "b", haverá um match?</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Sim, pois o 'a' pode aparecer zero vezes">Sim, pois o 'a' pode aparecer zero vezes</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Não, falta o 'a'</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas se ativar a flag global</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Não, pois Regex não aceita strings vazias
    > Resposta Correta: O `*` permite zero ocorrências de 'a'.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. O padrão `\w+` encontra qual destes?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">" " (um espaço)</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! "palavra"">"palavra"</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">"" (string vazia)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">"." (um ponto final)
    > Resposta Correta: `\w` encontra letras/números e o `+` exige ao menos um.</div>
  <div class="quiz-feedback"></div>
</div>

