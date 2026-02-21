# Quiz 08 - Introdução

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. Qual símbolo representa o operador de alternância ("OU")?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`&`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`+`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `|`">`|`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`!`
    > Resposta Correta: O `|` (pipe) é usado para alternar entre opções.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. O que o padrão `cachorro|gato` encontrará?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">A palavra "cachorrogato"</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Ou a palavra "cachorro" ou a palavra "gato"">Ou a palavra "cachorro" ou a palavra "gato"</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas animais domésticos</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Nada, dá erro de sintaxe
    > Resposta Correta: Ele age como uma escolha entre as duas palavras.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. Para que costumamos usar os parênteses em conjunto com a alternância?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Para mudar a cor do texto</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Para limitar o escopo da alternância a um trecho específico">Para limitar o escopo da alternância a um trecho específico</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Para desativar a alternância</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Para buscar apenas números
    > Resposta Correta: Ajuda a definir onde começa e termina o "OU" (ex: `A (B|C) D`).</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. No padrão `ab|abc`, qual o comportamento esperado ao encontrar o texto "abc"?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Ele sempre pegará "abc"</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Ele pode pegar apenas "ab" se o motor for do tipo que para no primeiro match satisfatório">Ele pode pegar apenas "ab" se o motor for do tipo que para no primeiro match satisfatório</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Ele dará erro de ambiguidade</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Ele pegará a letra "c"
    > Resposta Correta: Regex costuma ser "vanguardista" e pega a primeira opção válida da esquerda para a direita.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. O padrão `carro|moto` encontraria a palavra "carroça"?</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Sim, encontraria o trecho "carro" dentro de "carroça"">Sim, encontraria o trecho "carro" dentro de "carroça"</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Não, ele só busca palavras inteiras</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas se usar a flag global</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sim, mas apenas se a carroça for motorizada
    > Resposta Correta: Sem âncoras, o Regex busca partes de palavras.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. Como escrever um padrão que encontre "vermelho", "azul" ou "verde"?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`vermelho extra azul extra verde`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `vermelho|azul|verde`">`vermelho|azul|verde`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`[vermelho azul verde]`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`vermelho & azul & verde`
    > Resposta Correta: Basta separar as opções literais por `|`.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. O que o padrão `casa|` (com nada após o pipe) costuma fazer?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Dá erro de compilação</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Pode resultar em um "match vazio", o que é perigoso">Pode resultar em um "match vazio", o que é perigoso</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Busca apenas a palavra "casa"</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Busca o símbolo `|`
    > Resposta Correta: Um lado vazio da alternância pode casar com "nada" e causar loops ou matches inesperados.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. Para encontrar o símbolo literal `|` em um texto, o que devo fazer?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Digitar apenas `|`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Digitar `\|` (usar o escape)">Digitar `\|` (usar o escape)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Digitar `[|]`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Usar dois pipes `||`
    > Resposta Correta: Como é um metacaractere, precisa de escape.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. O padrão `(f|p)ato` dará match em quais palavras?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">fato e pato</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">rato e mato</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! apenas fato e pato">apenas fato e pato</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">f p ato
    > Resposta Correta: O grupo alterna apenas a primeira letra.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. A alternância `[a-z]|[0-9]` é redundante se eu puder usar:</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`\w`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`[a-z0-9]`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Ambas as opções acima são mais limpas">Ambas as opções acima são mais limpas</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Nenhuma, a alternância é a única forma
    > Resposta Correta: Conjuntos de caracteres costumam ser mais eficientes que a alternância para caracteres únicos.</div>
  <div class="quiz-feedback"></div>
</div>

