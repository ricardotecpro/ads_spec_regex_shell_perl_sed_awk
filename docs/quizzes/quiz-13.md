# Quiz 13 - Introdução

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. Qual a principal diferença entre Validação e Extração?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Nenhuma, são sinônimos</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Validação verifica se o todo está correto; Extração isola partes específicas">Validação verifica se o todo está correto; Extração isola partes específicas</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Validação é mais lenta</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Extração só funciona com nomes
    > Resposta Correta: Na extração, buscamos "matches" dentro de um texto maior.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. Em Python, qual função usamos para extrair uma LISTA de todos os matches?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`re.search()`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `re.findall()`">`re.findall()`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`re.extract()`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`re.sub()`
    > Resposta Correta: `findall` retorna todos os resultados em uma lista.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. Qual a função da flag `-o` no comando `grep` do terminal?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Abrir o arquivo</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Mostrar apenas a parte do texto que deu match (only matching)">Mostrar apenas a parte do texto que deu match (only matching)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Ocultar o resultado</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Ordenar os resultados
    > Resposta Correta: `-o` é fundamental para extrações rápidas no terminal.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. O padrão `#[a-zA-Z\d_]+` é ideal para extrair:</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">E-mails</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Hashtags de redes sociais">Hashtags de redes sociais</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Números de telefone</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Links de sites
    > Resposta Correta: Ele busca o símbolo `#` seguido de caracteres alfanuméricos.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. Ao usar parênteses em um padrão de extração, o que acontece no resultado do `match` ou `findall`?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">O Regex dá erro</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Ele retorna apenas o conteúdo que estava dentro dos parênteses (Grupo de Captura)">Ele retorna apenas o conteúdo que estava dentro dos parênteses (Grupo de Captura)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Ele ignora os parênteses</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Ele inverte o texto
    > Resposta Correta: Parênteses isolam o que você realmente quer extrair do resto do padrão.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. Como extrair todos os anos (4 dígitos) de um texto longo?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`\d{4}`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`[0-9]{4}`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Ambas as opções estão corretas">Ambas as opções estão corretas</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Nenhuma, precisa usar âncoras
    > Resposta Correta: Para extração, não usamos âncoras `^` e `$`, pois queremos encontrar no meio do texto.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. No padrão `href="([^"]+)"`, o que o conjunto `[^"]+` faz?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Busca apenas aspas</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Captura tudo o que NÃO for aspas (garantindo que ele pare na aspas de fechamento)">Captura tudo o que NÃO for aspas (garantindo que ele pare na aspas de fechamento)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Deleta o link</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Busca apenas letras
    > Resposta Correta: É uma técnica comum para capturar conteúdo entre delimitadores.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. Para extrair apenas o domínio de um e-mail (ex: `gmail.com`), qual o padrão correto?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`@.*`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `@([\w.]+)`">`@([\w.]+)`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`.*@`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`[a-z]+`
    > Resposta Correta: Captura tudo o que vem após o `@`.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. O Regex `[A-Z]{2}` extrairá a sigla "SP" da frase "Moro em SP"?</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Sim">Sim</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Não, falta a flag global</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas se "SP" estiver no final</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Não, Regex só busca palavras de 3 letras
    > Resposta Correta: Siglas de 2 letras maiúsculas darão match perfeitamente.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. Em uma busca por valores monetários `R\$ \d+`, o cifrão `$` precisa de escape?</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Sim, pois `$ sozinho` é a âncora de fim de linha">Sim, pois `$ sozinho` é a âncora de fim de linha</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Não, o Regex entende pelo contexto</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sim, mas apenas se estiver no final</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Não, pois é um símbolo de dinheiro
    > Resposta Correta: Metacaracteres devem ser escapados quando buscamos o símbolo literal.</div>
  <div class="quiz-feedback"></div>
</div>

