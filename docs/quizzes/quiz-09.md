# Quiz 09 - Introdução

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. O que são as Flags em Regex?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Símbolos usados dentro da expressão</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Modificadores que mudam o comportamento global da execução">Modificadores que mudam o comportamento global da execução</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Atalhos para números</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Erros de sintaxe
    > Resposta Correta: Elas definem COMO a expressão deve ser processada.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. Qual a função da flag `i`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Inserir texto</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Inverter a busca</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Ignorar a diferença entre maiúsculas e minúsculas">Ignorar a diferença entre maiúsculas e minúsculas</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Identificar números
    > Resposta Correta: "i" vem de case-insensitive.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. Sem a flag `g` (global), o que acontece em um texto com várias ocorrências de um padrão?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">O Regex encontra todas</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O Regex para após encontrar a primeira ocorrência">O Regex para após encontrar a primeira ocorrência</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">O Regex dá erro</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">O Regex encontra apenas a última
    > Resposta Correta: O comportamento padrão é parar no primeiro match.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. Para que serve a flag `m` (multiline)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Para buscar em vários arquivos ao mesmo tempo</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Para que `^` e `$` considerem cada linha individualmente">Para que `^` e `$` considerem cada linha individualmente</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Para permitir mais de um Regex na mesma linha</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Para formatar o texto em colunas
    > Resposta Correta: Muda o comportamento das âncoras de início e fim.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. O que a flag `s` (DotAll) permite ao metacaractere ponto (`.`)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Ser mais rápido</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Dar match em quebras de linha (`\n`)">Dar match em quebras de linha (`\n`)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Ser ignorado</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Só encontrar espaços
    > Resposta Correta: Normalmente o `.` ignora o caractere de nova linha.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. Onde as flags costumam ser posicionadas na sintaxe padrão?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">No início: `gi/padrao/`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! No final: `/padrao/gi`">No final: `/padrao/gi`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">No meio: `/pad/gi/rao`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Dentro dos colchetes
    > Resposta Correta: Elas vêm logo após o delimitador final.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. Qual flag é essencial para um comando de "Substituir Tudo" em um editor?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Flag `i`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Flag `g`">Flag `g`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Flag `m`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Flag `s`
    > Resposta Correta: Sem a flag global, apenas o primeiro item seria substituído.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. Se eu usar `/abc/i`, ele encontrará "ABC"?</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Sim, devido à flag de ignore case">Sim, devido à flag de ignore case</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Não, falta a flag global</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas se o texto estiver entre aspas</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Somente em JavaScript
    > Resposta Correta: A flag `i` resolve a diferença de caixa.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. A flag `u` (Unicode) é importante para:</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Deixar o código mais bonito</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Processar corretamente caracteres especiais, emojis e símbolos complexos">Processar corretamente caracteres especiais, emojis e símbolos complexos</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Traduzir o texto</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Aumentar o tamanho do arquivo
    > Resposta Correta: Garante o tratamento correto de caracteres multi-byte.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. Posso combinar várias flags juntas, como `gim`?</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Sim, elas se somam e aplicam todos os comportamentos ao mesmo tempo">Sim, elas se somam e aplicam todos os comportamentos ao mesmo tempo</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Não, deve-se usar apenas uma por vez</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sim, mas a ordem altera o resultado</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas em ferramentas de terminal
    > Resposta Correta: As flags podem ser combinadas livremente.</div>
  <div class="quiz-feedback"></div>
</div>

