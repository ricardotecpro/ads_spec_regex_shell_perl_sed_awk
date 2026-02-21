# Quiz 14 - Introdução

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. Qual o melhor uso do Regex no processo de sanitização de dados?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Criar novos bancos de dados</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Remover caracteres indesejados ou proibidos de um input">Remover caracteres indesejados ou proibidos de um input</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Traduzir o texto para outro idioma</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Aumentar o tamanho das fontes
    > Resposta Correta: Regex é excelente para remover "lixo" (caracteres especiais, espaços extras) de entradas de usuários.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. O padrão `\s{2,}` é usado para encontrar:</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Pelo menos dois números</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Dois ou mais espaços em branco seguidos">Dois ou mais espaços em branco seguidos</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Erros de ortografia</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Palavras com duas letras
    > Resposta Correta: Ajuda a identificar e remover espaços duplos.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. Como representamos a troca de posição entre dois grupos de captura na substituição?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`1$ 2$`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `$2 $1` (ou \2 \1)">`$2 $1` (ou \2 \1)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`swap(1,2)`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`{2}{1}`
    > Resposta Correta: A ordem dos identificadores de grupo define a nova ordem do texto.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. O padrão `^\s+|\s+$` serve para:</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Contar palavras</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Localizar espaços no início OU no fim do texto (Trim)">Localizar espaços no início OU no fim do texto (Trim)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Validar e-mails</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Deletar todo o texto
    > Resposta Correta: É a implementação manual do método "Trim" das linguagens.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. Ao transformar `2024-10-21` para `21/10/2024`, o Regex original deve ter quantos grupos de captura?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">1</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">2</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! 3 (Ano, Mês, Dia)">3 (Ano, Mês, Dia)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Nenhum
    > Resposta Correta: Cada parte da data precisa ser isolada para ser reordenada.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. O que o padrão `\D` faz em uma operação de limpeza de telefone?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Encontra apenas dígitos</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Encontra tudo o que NÃO é um dígito (parênteses, traços, espaços)">Encontra tudo o que NÃO é um dígito (parênteses, traços, espaços)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Exclui a linha inteira</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Formata o número
    > Resposta Correta: Útil para extrair apenas os números brutos.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. Qual a vantagem de usar Regex para converter nomes em "Slugs" de URL?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Deixa a URL colorida</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Automatiza a troca de caracteres especiais por hífens de forma padrão">Automatiza a troca de caracteres especiais por hífens de forma padrão</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Garante que o site suba no Google</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Protege contra hackers
    > Resposta Correta: Padroniza o formato de links de forma eficiente.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. No padrão `(<[^>]+>)`, o que estamos tentando encontrar?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Links de sites</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Imagens</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Qualquer tag HTML (para remoção ou extração)">Qualquer tag HTML (para remoção ou extração)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Comentários em Python
    > Resposta Correta: Busca o sinal de `<` seguido de qualquer coisa que não seja `>`, fechando em `>`.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. O método de substituição é destrutivo ou gera uma nova string?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Destrói a string original para sempre</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Geralmente gera uma nova string transformada, mantendo a original intacta">Geralmente gera uma nova string transformada, mantendo a original intacta</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Depende da cor do terminal</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Só funciona se houver match
    > Resposta Correta: Strings costumam ser imutáveis; a função retorna o resultado da transformação.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. Posso usar Regex para remover comentários de um código-fonte?</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Sim, identificando padrões como `//` ou `/* */`">Sim, identificando padrões como `//` ou `/* */`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Não, Regex não lê código</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apenas se o código estiver em JavaScript</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Sim, mas isso apagará todo o programa
    > Resposta Correta: É um uso clássico para limpeza de arquivos de configuração ou código.</div>
  <div class="quiz-feedback"></div>
</div>

