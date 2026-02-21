# Quiz 03 - Introdução

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. O que o metacaractere ponto (`.`) representa?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">O fim de uma frase</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Qualquer caractere único (exceto quebra de linha)">Qualquer caractere único (exceto quebra de linha)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas letras minúsculas</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas números
    > Resposta Correta: O ponto é o coringa universal para um único caractere.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. Qual atalho representa "qualquer dígito numérico"?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`\w`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`\s`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `\d`">`\d`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`\t`
    > Resposta Correta: `\d` vem de "digit".</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. O que o atalho `\w` captura?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas letras maiúsculas</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Letras, números e o caractere underline (`_`)">Letras, números e o caractere underline (`_`)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas símbolos especiais</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Somente espaços em branco
    > Resposta Correta: `\w` (word character) inclui alfanuméricos e `_`.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. Qual a função da barra invertida (`\`) antes de um metacaractere?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Excluir o caractere da busca</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Tornar a busca mais rápida</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Aplicar o "escape", buscando o caractere literal em vez do seu poder especial">Aplicar o "escape", buscando o caractere literal em vez do seu poder especial</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Mudar a cor do texto no editor
    > Resposta Correta: O escape desativa o metacaractere (ex: `\.`).</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. Se eu usar o padrão `\s`, o que encontrarei?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Símbolos de dinheiro</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Espaços, tabulações e quebras de linha">Espaços, tabulações e quebras de linha</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas a letra "s"</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Somente o início da frase
    > Resposta Correta: `\s` captura "whitespace" (espaços em branco).</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. O que representa a letra maiúscula nos atalhos, como `\D`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Uma busca mais forte</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! A negação (qualquer coisa que NÃO seja um dígito)">A negação (qualquer coisa que NÃO seja um dígito)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas letras em caixa alta</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Um erro de sintaxe
    > Resposta Correta: Maiúsculas costumam negar o atalho original.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. Para encontrar um endereço de IP como `127.0.0.1`, qual o Regex mais correto?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`127.0.0.1` (sem escape)</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `127\.0\.0\.1` (com escape)">`127\.0\.0\.1` (com escape)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`\d\d\d.\d.\d.\d`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`127*0*0*1`
    > Resposta Correta: O ponto real deve ser escapado para evitar que funcione como coringa.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. O padrão `c.sa` dará match em "coisa"?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sim, o ponto pega as letras "oi"</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Não, o ponto representa apenas UM caractere único">Não, o ponto representa apenas UM caractere único</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sim, ele ignora o número de letras</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Não, faltou o escape
    > Resposta Correta: Um ponto = um caractere. Para "oi" seriam necessários dois pontos.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. Qual atalho captura o espaço entre duas palavras em "Olá Mundo"?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`\d`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `\s`">`\s`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`\w`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`.` (apenas se for o último recurso)
    > Resposta Correta: `\s` é o específico para espaços.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. Como eu busco uma barra invertida literal (`\`) em um texto?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Digitando apenas `\`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Digitando `\\` (escapando a própria barra)">Digitando `\\` (escapando a própria barra)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Digitando `/`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Usando o ponto `.`
    > Resposta Correta: Como a barra é o caractere de escape, ela precisa escapar a si mesma.</div>
  <div class="quiz-feedback"></div>
</div>

