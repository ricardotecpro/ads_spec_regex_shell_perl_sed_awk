# Quiz 16 - Introdução

--8<-- "assets/quiz.html"

<div class="quiz-container">
  <div class="quiz-question">1. Qual o primeiro passo recomendado ao receber uma tarefa complexa de Regex?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Começar a digitar código imediatamente</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Testar o padrão e os dados de exemplo em uma ferramenta como Regex101">Testar o padrão e os dados de exemplo em uma ferramenta como Regex101</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Pedir para outra pessoa fazer</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Desistir e usar busca manual
    > Resposta Correta: Ferramentas de teste visual economizam muito tempo de depuração.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">2. O que aprendemos sobre a normalização de datas em Regex?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">É impossível fazer com Regex</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Datas não devem ter separadores</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Podemos usar grupos de captura para reordenar Dia, Mês e Ano">Podemos usar grupos de captura para reordenar Dia, Mês e Ano</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Regex só aceita o formato americano
    > Resposta Correta: Grupos e substituição são perfeitos para mudar formatos.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">3. Para normalizar "Pago", "pago" e "PAGO" em um único padrão, qual a melhor estratégia?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Escrever as três opções separadas por `|`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Usar a palavra `pago` com a flag `i` (ignore case)">Usar a palavra `pago` com a flag `i` (ignore case)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Usar o ponto `.`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Não há como fazer
    > Resposta Correta: A flag `i` simplifica muito a busca por palavras com variação de caixa.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">4. Se o seu projeto final precisa extrair IPs, qual classe de caractere é a mais adequada?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`\w`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `\d` (pois IPs são compostos por dígitos e pontos)">`\d` (pois IPs são compostos por dígitos e pontos)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`\s`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`\A`
    > Resposta Correta: `\d` ou `[0-9]` são essenciais para encontrar números.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">5. Em um script de limpeza, por que limpamos caracteres não-numéricos antes de salvar no banco?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Para o banco ficar mais bonito</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Para garantir integridade dos dados e facilitar cálculos futuros">Para garantir integridade dos dados e facilitar cálculos futuros</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Para o arquivo pesar mais</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">É apenas uma tradição
    > Resposta Correta: Dados limpos e padronizados evitam erros de processamento e lógica.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">6. Qual metacaractere foi o mais versátil ao longo do curso para buscas rápidas?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`$`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`^`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `.` (Ponto)">`.` (Ponto)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`\`
    > Resposta Correta: O ponto é o coringa para qualquer caractere único.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">7. No seu projeto final, se você quiser garantir que o Regex pegue o nome de usuário até o símbolo `|`, o que deve usar?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`.*|`</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! `.*?\|` (Preguiçoso com escape da barra)">`.*?\|` (Preguiçoso com escape da barra)</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`.+`</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">`^$`
    > Resposta Correta: O modo preguiçoso evita que o Regex pegue mais do que o necessário.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">8. O que significa "Refatorar um Regex"?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Apagar e começar do zero</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Melhorar o padrão existente para torná-lo mais legível ou performático">Melhorar o padrão existente para torná-lo mais legível ou performático</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Mudar a linguagem de programação</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Adicionar mais erros
    > Resposta Correta: Refatoração foca em qualidade e eficiência.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">9. Após terminar este curso, você se sente apto a:</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Hackear a NASA</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! Enfrentar desafios de manipulação e validação de texto com confiança">Enfrentar desafios de manipulação e validação de texto com confiança</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Criar uma nova linguagem de programação</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Parar de usar computador
    > Resposta Correta: O objetivo foi dar autonomia e ferramentas para lidar com dados de texto.</div>
  <div class="quiz-feedback"></div>
</div>

<div class="quiz-container">
  <div class="quiz-question">10. Qual a mensagem final do curso sobre Expressões Regulares?</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Elas são inúteis</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">Devem ser evitadas a todo custo</div>
  <div class="quiz-option" data-correct="true" data-feedback="✅ Correto! São um superpoder que, se usado com sabedoria e boas práticas, aumenta muito a produtividade">São um superpoder que, se usado com sabedoria e boas práticas, aumenta muito a produtividade</div>
  <div class="quiz-option" data-correct="false" data-feedback="Incorreto. Tente novamente.">São apenas para quem gosta de matemática
    > Resposta Correta: Regex é uma ferramenta essencial e poderosa no arsenal de qualquer profissional de TI.</div>
  <div class="quiz-feedback"></div>
</div>

