# Quiz 07 - Agrupamentos e Captura 🎯

1. Qual símbolo usamos para criar um grupo de captura?
    - [ ] `[]`
    - [ ] `{}`
    - [x] `()`
    - [ ] `<>`
    > Resposta Correta: Parênteses são usados para agrupar e capturar.

2. Qual a principal diferença entre `[abc]` e `(abc)`?
    - [ ] Não há diferença
    - [x] `[abc]` busca uma letra; `(abc)` busca a sequência exata "abc"
    - [ ] O primeiro é mais rápido
    - [ ] O segundo é apenas para números
    > Resposta Correta: Colchetes são conjuntos (OU); Parênteses são grupos (SEQUÊNCIA).

3. Como nos referimos ao primeiro grupo de captura dentro da própria expressão?
    - [ ] `$1`
    - [ ] `#1`
    - [x] `\1`
    - [ ] group(1)
    > Resposta Correta: Usamos a barra invertida seguida do número do grupo (Backreference).

4. O que acontece se aplicarmos um quantificador a um grupo, como `(ha){3}`?
    - [ ] Ele busca "ha" e depois o número 3
    - [x] Ele busca a sequência "hahaha"
    - [ ] Ele busca "ha" no máximo 3 vezes
    - [ ] Dá erro de sintaxe
    > Resposta Correta: O quantificador repete todo o conteúdo do grupo.

5. Qual grupo representa o "Match completo" (todo o texto encontrado)?
    - [x] Grupo 0
    - [ ] Grupo 1
    - [ ] Grupo Final
    - [ ] O Regex não numera o match completo
    > Resposta Correta: O Grupo 0 sempre contém o resultado total da expressão.

6. Quantos grupos de captura existem no padrão `(\d+)-(\w+)-(\s+)`?
    - [ ] 1
    - [ ] 2
    - [x] 3
    - [ ] 6
    > Resposta Correta: Cada par de parênteses cria um grupo novo.

7. Em um motor de substituição (como VS Code ou sed), como costumamos chamar o conteúdo do Grupo 1?
    - [ ] `\1` ou `$1`
    - [ ] `Group1`
    - [ ] `%1`
    - [ ] `{1}`
    > Resposta Correta: Geralmente `$1` ou `\1` dependendo da linguagem.

8. Para que serve o grupo de "não-captura" `(?:...)`?
    - [ ] Para esconder a senha
    - [x] Para agrupar sem salvar o resultado na memória (economiza performance)
    - [ ] Para comentar o código
    - [ ] Para ignorar maiúsculas
    > Resposta Correta: Útil quando você quer apenas agrupar, mas não precisa extrair o dado depois.

9. O padrão `(\w)\1` encontrará qual destes textos?
    - [ ] ab
    - [x] aa
    - [ ] a1
    - [ ] a
    > Resposta Correta: Ele encontrará qualquer caractere seguido dele mesmo (repetição).

10. Como a numeração de grupos é decidida em grupos aninhados como `((A)B)`?
    - [ ] Pela importância
    - [x] Pela ordem de abertura dos parênteses (Grupo 1 é o externo, Grupo 2 é o interno)
    - [ ] Aleatoriamente
    - [ ] De dentro para fora
    > Resposta Correta: O primeiro `(` que abre define o Grupo 1.