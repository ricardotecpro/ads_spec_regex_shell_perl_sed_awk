# Quiz 08 - Alternância 🔀

1. Qual símbolo representa o operador de alternância ("OU")?
    - [ ] `&`
    - [ ] `+`
    - [x] `|`
    - [ ] `!`
    > Resposta Correta: O `|` (pipe) é usado para alternar entre opções.

2. O que o padrão `cachorro|gato` encontrará?
    - [ ] A palavra "cachorrogato"
    - [x] Ou a palavra "cachorro" ou a palavra "gato"
    - [ ] Apenas animais domésticos
    - [ ] Nada, dá erro de sintaxe
    > Resposta Correta: Ele age como uma escolha entre as duas palavras.

3. Para que costumamos usar os parênteses em conjunto com a alternância?
    - [ ] Para mudar a cor do texto
    - [x] Para limitar o escopo da alternância a um trecho específico
    - [ ] Para desativar a alternância
    - [ ] Para buscar apenas números
    > Resposta Correta: Ajuda a definir onde começa e termina o "OU" (ex: `A (B|C) D`).

4. No padrão `ab|abc`, qual o comportamento esperado ao encontrar o texto "abc"?
    - [ ] Ele sempre pegará "abc"
    - [x] Ele pode pegar apenas "ab" se o motor for do tipo que para no primeiro match satisfatório
    - [ ] Ele dará erro de ambiguidade
    - [ ] Ele pegará a letra "c"
    > Resposta Correta: Regex costuma ser "vanguardista" e pega a primeira opção válida da esquerda para a direita.

5. O padrão `carro|moto` encontraria a palavra "carroça"?
    - [x] Sim, encontraria o trecho "carro" dentro de "carroça"
    - [ ] Não, ele só busca palavras inteiras
    - [ ] Apenas se usar a flag global
    - [ ] Sim, mas apenas se a carroça for motorizada
    > Resposta Correta: Sem âncoras, o Regex busca partes de palavras.

6. Como escrever um padrão que encontre "vermelho", "azul" ou "verde"?
    - [ ] `vermelho extra azul extra verde`
    - [x] `vermelho|azul|verde`
    - [ ] `[vermelho azul verde]`
    - [ ] `vermelho & azul & verde`
    > Resposta Correta: Basta separar as opções literais por `|`.

7. O que o padrão `casa|` (com nada após o pipe) costuma fazer?
    - [ ] Dá erro de compilação
    - [x] Pode resultar em um "match vazio", o que é perigoso
    - [ ] Busca apenas a palavra "casa"
    - [ ] Busca o símbolo `|`
    > Resposta Correta: Um lado vazio da alternância pode casar com "nada" e causar loops ou matches inesperados.

8. Para encontrar o símbolo literal `|` em um texto, o que devo fazer?
    - [ ] Digitar apenas `|`
    - [x] Digitar `\|` (usar o escape)
    - [ ] Digitar `[|]`
    - [ ] Usar dois pipes `||`
    > Resposta Correta: Como é um metacaractere, precisa de escape.

9. O padrão `(f|p)ato` dará match em quais palavras?
    - [ ] fato e pato
    - [ ] rato e mato
    - [x] apenas fato e pato
    - [ ] f p ato
    > Resposta Correta: O grupo alterna apenas a primeira letra.

10. A alternância `[a-z]|[0-9]` é redundante se eu puder usar:
    - [ ] `\w`
    - [ ] `[a-z0-9]`
    - [x] Ambas as opções acima são mais limpas
    - [ ] Nenhuma, a alternância é a única forma
    > Resposta Correta: Conjuntos de caracteres costumam ser mais eficientes que a alternância para caracteres únicos.