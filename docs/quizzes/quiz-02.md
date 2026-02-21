# Quiz 02 - Introdução

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. O que é uma busca literal em Regex?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Uma busca que tenta adivinhar o que você quer</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Uma busca por uma sequência exata de caracteres fixos">Uma busca por uma sequência exata de caracteres fixos</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Uma busca que só funciona com números</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Uma busca que ignora espaços
    > Resposta Correta: Busca literal procura por caracteres exatos na ordem especificada.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. Se eu buscar pelo padrão "gato", qual destes textos terá um match?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Gato</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">GATO</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! sapato">sapato</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">cachorro
    > Resposta Correta: "sapato" contém a sequência literal "gato". Sem flags, o Regex diferencia maiúsculas.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. O que significa a característica "Case-Sensitive"?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Que o Regex é sensível a espaços</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Que existe diferença entre letras maiúsculas e minúsculas">Que existe diferença entre letras maiúsculas e minúsculas</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Que o Regex não aceita acentos</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Que a busca é mais lenta
    > Resposta Correta: É a distinção entre caracteres 'A' e 'a'.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. Qual "Flag" (modificador) deve ser usada para tornar a busca case-insensitive?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Flag `g`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Flag `i`">Flag `i`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Flag `m`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Flag `s`
    > Resposta Correta: A flag `i` vem de "Ignore case".</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. Ao buscar "casa ", com um espaço no final, o Regex encontrará a palavra "casa" (sem espaço)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sim, ele ignora espaços extras</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Não, o espaço é considerado um caractere literal e deve estar presente">Não, o espaço é considerado um caractere literal e deve estar presente</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Depende da linguagem de programação</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas se for no final da linha
    > Resposta Correta: Espaços são caracteres literais em Regex.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. O padrão "123" encontrará o número "123" em uma string como "ID_12345"?</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Sim, pois a sequência literal está contida na string">Sim, pois a sequência literal está contida na string</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Não, ele só busca palavras completas</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas se for o início da string</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Não, números não podem ser buscados literalmente
    > Resposta Correta: O match ocorre na parte da string que corresponde ao padrão.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. Qual a diferença entre "CASA" (padrão) e "casa" (texto) sem flags?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">São idênticos para o Regex</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O Regex não encontrará correspondência (No match)">O Regex não encontrará correspondência (No match)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">O Regex encontrará apenas as letras "A"</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">O computador emitirá um alerta de erro
    > Resposta Correta: Sem a flag `i`, o padrão e o texto devem ter a mesma caixa.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. Posso usar acentos em uma busca literal, como "maçã"?</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Sim, caracteres acentuados são tratados como caracteres literais normais">Sim, caracteres acentuados são tratados como caracteres literais normais</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Não, Regex não suporta caracteres especiais da língua portuguesa</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sim, mas o Regex101 não mostra</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas se você converter para código ASCII
    > Resposta Correta: Acentos são suportados perfeitamente.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. Se eu buscar por " " (dois espaços), o que o Regex encontrará?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas uma quebra de linha</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Nada, espaços não são pesquisáveis</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Exatamente duas ocorrências de espaços seguidos">Exatamente duas ocorrências de espaços seguidos</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Qualquer lugar onde falte um caractere
    > Resposta Correta: Espaços seguidos formam um padrão literal válido.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. No Regex101, onde as "Flags" geralmente são configuradas?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">No meio do texto de teste</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Elas não existem no site</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! No canto superior direito, ao lado da barra de expressão">No canto superior direito, ao lado da barra de expressão</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">No rodapé da página
    > Resposta Correta: Existe um ícone de bandeira ou um campo específico para flags (ex: `/padrão/gi`).</div>
  <div class="quiz-feedback"></div>
</div>

