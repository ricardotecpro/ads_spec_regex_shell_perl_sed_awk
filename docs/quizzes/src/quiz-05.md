# Quiz 05 - Quantificadores 🔢

1. Qual símbolo representa "zero ou mais ocorrências"?
    - [ ] `+`
    - [ ] `?`
    - [x] `*`
    - [ ] `{0}`
    > Resposta Correta: O asterisco `*` permite que o padrão apareça nunca ou muitas vezes.

2. Qual a diferença entre `*` e `+`?
    - [ ] `*` é para números e `+` para letras
    - [x] `+` exige ao menos uma ocorrência; `*` aceita zero
    - [ ] `*` é mais rápido
    - [ ] Não há diferença
    > Resposta Correta: O sinal de mais `+` significa "um ou mais".

3. O que o quantificador `{3}` faz?
    - [ ] Busca o número 3 no texto
    - [x] Faz com que o padrão anterior se repita exatamente 3 vezes
    - [ ] Busca no máximo 3 vezes
    - [ ] Indica a terceira linha do arquivo
    > Resposta Correta: Define uma quantidade exata de repetições.

4. Como escrevemos um padrão que aceite de 2 a 5 dígitos?
    - [ ] `\d{2-5}`
    - [x] `\d{2,5}`
    - [ ] `\d(2,5)`
    - [ ] `\d[2-5]`
    > Resposta Correta: A sintaxe correta usa vírgula `{m,n}`.

5. O que significa o símbolo `?` quando usado sozinho após um caractere?
    - [ ] Uma pergunta ao motor de busca
    - [x] Que o caractere anterior é opcional (zero ou uma vez)
    - [ ] Que o texto é um link
    - [ ] Que a busca deve parar
    > Resposta Correta: O ponto de interrogação torna o item anterior opcional.

6. O que é um quantificador "Guloso" (Greedy)?
    - [ ] Um que trava o computador
    - [x] Um que tenta capturar o maior trecho de texto possível
    - [ ] Um que só busca palavras longas
    - [ ] Um que ignora espaços
    > Resposta Correta: Ele consome o máximo de caracteres que casam com o padrão.

7. Como transformamos um quantificador guloso (como `.*`) em "Preguiçoso" (Lazy)?
    - [ ] Usando a flag `/L`
    - [ ] Colocando um `+` no final
    - [x] Colocando um `?` logo após o quantificador (ex: `.*?`)
    - [ ] Diminuindo o tamanho do texto
    > Resposta Correta: O `?` após outro quantificador muda seu comportamento para o mínimo possível.

8. O padrão `[0-9]{2,}` significa:
    - [ ] Exatamente 2 números
    - [ ] No máximo 2 números
    - [x] No mínimo 2 números (sem limite superior)
    - [ ] Números que terminam com vírgula
    > Resposta Correta: Deixando o segundo valor vazio `{2,}`, remove-se o limite máximo.

9. Se eu buscar `ba*` no texto "b", haverá um match?
    - [x] Sim, pois o 'a' pode aparecer zero vezes
    - [ ] Não, falta o 'a'
    - [ ] Apenas se ativar a flag global
    - [ ] Não, pois Regex não aceita strings vazias
    > Resposta Correta: O `*` permite zero ocorrências de 'a'.

10. O padrão `\w+` encontra qual destes?
    - [ ] " " (um espaço)
    - [x] "palavra"
    - [ ] "" (string vazia)
    - [ ] "." (um ponto final)
    > Resposta Correta: `\w` encontra letras/números e o `+` exige ao menos um.