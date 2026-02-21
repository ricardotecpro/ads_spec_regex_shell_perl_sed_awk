# Quiz 06 - Introdução

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. O que a âncora `^` representa (fora de colchetes)?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">O fim da linha</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! O início da linha ou do texto">O início da linha ou do texto</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Uma negação</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Um caractere especial
    > Resposta Correta: O `^` ancora a busca no começo da linha.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. Qual símbolo usamos para indicar o fim de uma linha?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`^`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`#`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `$`">`$`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`&`
    > Resposta Correta: O cifrão `$` ancora a busca no final da linha.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. Por que usamos `^` e `$` juntos em validação de formulários?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Para economizar memória</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Para garantir que o padrão preencha a linha inteira, sem extras">Para garantir que o padrão preencha a linha inteira, sem extras</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Para permitir qualquer caractere no meio</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Para transformar o texto em maiúsculas
    > Resposta Correta: Garante que o input atenda exatamente à regra do início ao fim.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. O padrão `^abc` encontrará a palavra "abc" em "123abc"?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sim, ele ignora o início</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Não, pois "abc" não está no início da string">Não, pois "abc" não está no início da string</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sim, mas apenas se usar a flag global</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas em sistemas Windows
    > Resposta Correta: A busca falha porque o início da string é "1".</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. O padrão `xyz$` dará match no texto "arquivo_xyz.txt"?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sim, contém xyz</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Não, pois a string termina com ".txt" e não com "xyz"">Não, pois a string termina com ".txt" e não com "xyz"</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sim, mas apenas o "xyz"</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Depende do editor de texto
    > Resposta Correta: A âncora `$` exige que o padrão seja o último item.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. Qual o efeito da flag `m` (multiline) nas âncoras?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Desativa as âncoras</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Faz com que `^` e `$` funcionem para CADA linha de um texto, e não apenas o texto todo">Faz com que `^` e `$` funcionem para CADA linha de um texto, e não apenas o texto todo</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Permite buscar em múltiplos arquivos</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Mudar o idioma do motor Regex
    > Resposta Correta: Trata cada quebra de linha como um novo início/fim.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. O padrão `^\d{3}$` aceita o texto "1234"?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sim, contém 3 dígitos</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Não, pois a linha inteira deve ter exatamente 3 dígitos">Não, pois a linha inteira deve ter exatamente 3 dígitos</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sim, mas ignora o último número</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas se houver um espaço depois
    > Resposta Correta: O padrão exige 3 dígitos e o fim da linha logo após.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. Se eu quiser encontrar uma linha vazia (sem nenhum caractere), qual o padrão?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">` ` (espaço)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`.*`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `^$`">`^$`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`\s`
    > Resposta Correta: Início seguido imediatamente pelo fim significa vazio.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. O padrão `^$` daria match em um texto com um único espaço?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sim</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Não, pois o espaço é um caractere e estaria entre o início e o fim">Não, pois o espaço é um caractere e estaria entre o início e o fim</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas se for no Linux</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sim, pois espaço é invisível
    > Resposta Correta: O espaço impediria o match de `^$`.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. No Regex, o símbolo `^` dentro de `[]` (como em `[^0-9]`) tem o mesmo sentido de âncora?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sim, sempre</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Não, dentro de colchetes ele significa negação">Não, dentro de colchetes ele significa negação</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas se for a primeira letra</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sim, mas apenas em JavaScript
    > Resposta Correta: O contexto muda completamente o significado do símbolo.</div>
  <div class="quiz-feedback"></div>
</div>

