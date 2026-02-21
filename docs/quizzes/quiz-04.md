# Quiz 04 - Introdução

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. Para que servem os colchetes `[]` em Regex?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Para indicar um comentário</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Para definir um conjunto de caracteres permitidos em uma posição">Para definir um conjunto de caracteres permitidos em uma posição</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Para agrupar expressões complexas</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Para marcar o início do texto
    > Resposta Correta: Os colchetes permitem escolher UM entre vários caracteres listados.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. O padrão `[aeiou]` encontrará qual destes?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">A palavra "aeiou" inteira</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Qualquer vogal individual minúscula">Qualquer vogal individual minúscula</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas a letra "a"</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Qualquer letra do alfabeto
    > Resposta Correta: Encontrará 'a', 'e', 'i', 'o' ou 'u' individualmente.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. Como representamos o intervalo de todas as letras minúsculas de forma curta?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`[a,z]`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`[a..z]`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `[a-z]`">`[a-z]`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`[a:z]`
    > Resposta Correta: O hífen `-` define o intervalo (range).</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. O que o conjunto `[0-9]` representa?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas os números 0 e 9</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Qualquer algarismo de 0 a 9 (o mesmo que \d)">Qualquer algarismo de 0 a 9 (o mesmo que \d)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">O resultado de uma conta de subtração</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Uma data
    > Resposta Correta: Representa a classe dos dígitos decimais.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. Qual símbolo é usado para NEGAR um conjunto quando colocado no início dos colchetes?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`!`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`-`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `^`">`^`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`*`
    > Resposta Correta: O circunflexo no início nega o conjunto (ex: `[^...]`).</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. O padrão `[a-zA-Z]` encontrará qual tipo de caractere?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas letras com acento</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Qualquer letra latina, seja maiúscula ou minúscula">Qualquer letra latina, seja maiúscula ou minúscula</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas as letras 'a' e 'z'</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Letras e números misturados
    > Resposta Correta: Combina dois intervalos de letras.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. Se eu usar `[^0-9]`, o que terei como resultado?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas números negativos</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Qualquer caractere que NÃO seja um número">Qualquer caractere que NÃO seja um número</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">O número 0 e o número 9</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Um erro de código
    > Resposta Correta: É a negação dos dígitos.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. O conjunto `[123]` é diferente de `[1-3]`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sim, o primeiro busca o número 123</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Não, ambos buscam individualmente os números 1, 2 ou 3">Não, ambos buscam individualmente os números 1, 2 ou 3</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sim, o segundo é mais lento</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sim, o primeiro só aceita o número 1
    > Resposta Correta: Ambos representam os mesmos caracteres individuais.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. Onde o hífen `-` deve ser colocado se eu quiser pesquisá-lo literalmente dentro de um conjunto sem que ele crie um intervalo?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">No meio das letras</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! No início ou no fim do conjunto (ex: `[-az]` ou `[az-]`)">No início ou no fim do conjunto (ex: `[-az]` ou `[az-]`)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sempre fora dos colchetes</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Ele não pode ser pesquisado em conjuntos
    > Resposta Correta: Nas extremidades ele perde o poder de definir intervalo.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. O padrão `[A-Z][0-9]` daria match em qual destes textos?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">a1</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! B3">B3</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">9Z</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">AB
    > Resposta Correta: Primeiro caractere Maiúscula, segundo um Número.</div>
  <div class="quiz-feedback"></div>
</div>

