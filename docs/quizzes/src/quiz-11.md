# Quiz 11 - Regex com Python 🐍

1. Qual biblioteca do Python é usada para trabalhar com Expressões Regulares?
    - [ ] `regex`
    - [x] `re`
    - [ ] `math`
    - [ ] `os`
    > Resposta Correta: O módulo `re` é a biblioteca padrão.

2. O que significa o prefixo `r` em uma string Regex (ex: `r"\d"`)?
    - [ ] Read-only
    - [x] Raw String (String Bruta), preservando as barras invertidas
    - [ ] Replace mode
    - [ ] Regex mode
    > Resposta Correta: Evita que o Python interprete escapes como `\n` ou `\t`.

3. Qual função encontra a PRIMEIRA ocorrência de um padrão em uma string?
    - [ ] `re.findall()`
    - [x] `re.search()`
    - [ ] `re.match()`
    - [ ] `re.sub()`
    > Resposta Correta: `re.search()` varre a string toda em busca da primeira chance.

4. Qual a diferença entre `re.match()` e `re.search()` no Python?
    - [ ] Nenhuma
    - [x] `match` só procura no INÍCIO da string; `search` procura em QUALQUER lugar
    - [ ] `search` é mais rápido
    - [ ] `match` retorna uma lista
    > Resposta Correta: `re.match()` é implícitamente ancorado no começo.

5. Qual função retorna uma LISTA com todos os matches encontrados?
    - [ ] `re.list()`
    - [ ] `re.search_all()`
    - [x] `re.findall()`
    - [ ] `re.extract()`
    > Resposta Correta: `findall()` é ideal para extrair coleções de dados.

6. Como substituímos um padrão por outro texto usando o módulo `re`?
    - [ ] `re.replace()`
    - [ ] `re.change()`
    - [x] `re.sub()`
    - [ ] `re.swap()`
    > Resposta Correta: `sub` vem de "substitute".

7. O que a função `re.findall()` retorna se não encontrar nenhuma ocorrência?
    - [ ] `None`
    - [x] Uma lista vazia `[]`
    - [ ] Um erro de sistema
    - [ ] `False`
    > Resposta Correta: Retorna uma lista vazia, facilitando loops `for`.

8. Para acessar o conteúdo capturado por um grupo em `re.search()`, usamos:
    - [ ] `.content()`
    - [x] `.group()` ou `.groups()`
    - [ ] `.text()`
    - [ ] `[0]`
    > Resposta Correta: O objeto Match possui o método `.group()`.

9. No Python, as flags (como IgnoreCase) são passadas como:
    - [ ] `/padrao/i`
    - [x] Um argumento opcional: `re.search(p, s, flags=re.IGNORECASE)`
    - [ ] Não existem flags no Python
    - [ ] No início do padrão: `(i)padrao`
    > Resposta Correta: São passadas através do argumento `flags` usando constantes do módulo `re`.

10. O padrão `re.split(r"\s+", texto)` resultará em:
    - [ ] Uma string sem espaços
    - [x] Uma lista de palavras separadas pelos espaços
    - [ ] Um erro de tipo
    - [ ] Apenas o primeiro espaço
    > Resposta Correta: `split` divide a string baseada no padrão Regex.