# Quiz 10 - Regex com JavaScript 📜

1. Qual a forma mais comum de declarar um Regex literal em JavaScript?
    - [ ] `new RegExp("padrao")`
    - [x] `/padrao/`
    - [ ] `regex("padrao")`
    - [ ] `"padrao".toRegex()`
    > Resposta Correta: A sintaxe entre barras `/.../` é a mais utilizada.

2. Qual método do objeto Regex retorna apenas `true` ou `false`?
    - [ ] `.match()`
    - [ ] `.search()`
    - [x] `.test()`
    - [ ] `.exec()`
    > Resposta Correta: `.test()` é ideal para validações booleanas.

3. Onde o método `.match()` deve ser chamado?
    - [ ] No objeto Regex (`regex.match(texto)`)
    - [x] Na própria String (`texto.match(regex)`)
    - [ ] Globalmente
    - [ ] No console
    > Resposta Correta: `.match()` é um método do protótipo de String.

4. O que o método `.match()` retorna quando não encontra nada?
    - [ ] Um array vazio `[]`
    - [ ] `false`
    - [x] `null`
    - [ ] `undefined`
    > Resposta Correta: No JavaScript, se não houver match, o retorno é `null`.

5. Qual método usamos para substituir textos usando Regex no JavaScript?
    - [ ] `.change()`
    - [x] `.replace()`
    - [ ] `.substitute()`
    - [ ] `.map()`
    > Resposta Correta: `.replace()` aceita tanto strings simples quanto Regex.

6. O que a flag `g` faz no método `.replace()`?
    - [ ] Nada, ela é ignorada
    - [ ] Substitui apenas a primeira ocorrência
    - [x] Garante que TODAS as ocorrências sejam substituídas
    - [ ] Torna a substituição invisível
    > Resposta Correta: Sem o `g`, o JavaScript substitui apenas a primeira por padrão.

7. Como passamos flags ao criar um Regex com `new RegExp()`?
    - [ ] `/padrao/gi`
    - [x] `new RegExp("padrao", "gi")` (como segundo argumento)
    - [ ] `new RegExp("padrao/gi")`
    - [ ] Não é possível passar flags
    > Resposta Correta: O segundo parâmetro da função construtora aceita as flags.

8. O padrão `/\d+/` dará match em qual valor do objeto `test("Aula 10")`?
    - [ ] "Aula"
    - [ ] " " (espaço)
    - [x] true
    - [ ] 10
    > Resposta Correta: O método `.test()` retorna booleano, e como há números, retornará `true`.

9. O método `.replaceAll()` (adicionado recentemente no JS) exige que o Regex tenha qual flag?
    - [ ] Flag `i`
    - [x] Flag `g`
    - [ ] Flag `m`
    - [ ] Não exige nenhuma flag
    > Resposta Correta: O `replaceAll` com Regex lança erro se a flag global não estiver presente.

10. Qual a principal vantagem de usar Regex literais em vez do construtor `new RegExp()`?
    - [ ] É mais lento
    - [x] É mais legível e processado mais rápido pelo motor JS (estático)
    - [ ] Aceita variáveis dentro dele
    - [ ] Não precisa de barras
    > Resposta Correta: Literais são analisados no momento do carregamento do script.