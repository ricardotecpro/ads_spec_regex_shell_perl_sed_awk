# Quiz 15 - Introdução

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. O que é o "Catastrophic Backtracking"?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Um erro de digitação</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Um estado onde o motor Regex tenta bilhões de combinações, travando o sistema">Um estado onde o motor Regex tenta bilhões de combinações, travando o sistema</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Quando o Regex volta para o início do arquivo</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Uma flag de segurança
    > Resposta Correta: Ocorre em padrões complexos (geralmente quantificadores aninhados).</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. Qual destes padrões é considerado perigoso para a performance?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`[a-z]+`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`^\d+$`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `(a+)+b`">`(a+)+b`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`\s?`
    > Resposta Correta: O aninhamento de `+` dentro de outro `+` cria uma explosão combinatória.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. Por que usar `(?:...)` em vez de `(...)`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">É mais bonito</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Melhora a performance ao evitar que o motor salve o match na memória (não-captura)">Melhora a performance ao evitar que o motor salve o match na memória (não-captura)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">É a única forma de usar o OU `|`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Não há diferença real
    > Resposta Correta: Grupos de não-captura são mais leves para o sistema.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. Em termos de performance, o que é melhor: `.*` ou `[0-9]+`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`.*`, pois é o mais versátil</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `[0-9]+`, pois é mais específico e evita buscas desnecessárias">`[0-9]+`, pois é mais específico e evita buscas desnecessárias</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Dão no mesmo</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Nenhum, use apenas letras
    > Resposta Correta: Quanto mais específico for o padrão, menos o motor precisa "adivinhar".</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. Para que servem as ferramentas de "Debugger" no Regex101?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Para traduzir o Regex</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Para ver passo a passo como o motor está tentando encontrar o match e onde ele falha">Para ver passo a passo como o motor está tentando encontrar o match e onde ele falha</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Para salvar o Regex na nuvem</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Para criar gráficos coloridos
    > Resposta Correta: Essencial para identificar gargalos de performance.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. O que significa "ReDoS"?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Redo Operation Software</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Regular Expression Denial of Service (Ataque de negação de serviço via Regex)">Regular Expression Denial of Service (Ataque de negação de serviço via Regex)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Regex Data System</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Registro de Dados Online
    > Resposta Correta: É um ataque que explora Regex lentos para derrubar servidores.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. Por que devemos usar âncoras (`^` e `$`) sempre que possível?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Para deixar o padrão mais longo</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Para limitar o espaço de busca e permitir que o motor falhe rápido se o início não bater">Para limitar o espaço de busca e permitir que o motor falhe rápido se o início não bater</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Porque é uma regra obrigatória do JavaScript</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Para mudar o idioma da busca
    > Resposta Correta: Âncoras reduzem drasticamente o número de tentativas do motor.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. Qual a melhor prática para lidar com expressões muito complexas e longas?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Escrever tudo em uma única linha gigante</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Comentar o código e, se a linguagem permitir, usar o modo "verbose" (com espaços e comentários)">Comentar o código e, se a linguagem permitir, usar o modo "verbose" (com espaços e comentários)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Evitar usar Regex e fazer tudo com `if/else`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Usar apenas letras minúsculas
    > Resposta Correta: Documentação é vital para a manutenção do código.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. Na alternância `A|B|C`, onde deve ficar o padrão mais frequente?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">No final</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">No meio</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! No início (da esquerda para a direita)">No início (da esquerda para a direita)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Não importa a ordem
    > Resposta Correta: O motor para no primeiro match satisfatório; colocar o comum primeiro economiza tempo.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. Usar Regex é sempre a solução mais rápida para qualquer problema de string?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sim, Regex é imbatível</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Não, para buscas muito simples (tipo `indexOf` ou `startsWith`), métodos nativos de string são mais rápidos">Não, para buscas muito simples (tipo `indexOf` ou `startsWith`), métodos nativos de string são mais rápidos</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas em Python</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sim, mas apenas no Linux
    > Resposta Correta: Use a ferramenta certa para o trabalho. Regex tem um custo de "compilação" inicial.</div>
  <div class="quiz-feedback"></div>
</div>

