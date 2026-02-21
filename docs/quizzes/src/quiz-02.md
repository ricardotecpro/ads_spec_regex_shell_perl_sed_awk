# Quiz 02 - Estrutura Básica 🏗️

1. O que é uma busca literal em Regex?
    - [ ] Uma busca que tenta adivinhar o que você quer
    - [x] Uma busca por uma sequência exata de caracteres fixos
    - [ ] Uma busca que só funciona com números
    - [ ] Uma busca que ignora espaços
    > Resposta Correta: Busca literal procura por caracteres exatos na ordem especificada.

2. Se eu buscar pelo padrão "gato", qual destes textos terá um match?
    - [ ] Gato
    - [ ] GATO
    - [x] sapato
    - [ ] cachorro
    > Resposta Correta: "sapato" contém a sequência literal "gato". Sem flags, o Regex diferencia maiúsculas.

3. O que significa a característica "Case-Sensitive"?
    - [ ] Que o Regex é sensível a espaços
    - [x] Que existe diferença entre letras maiúsculas e minúsculas
    - [ ] Que o Regex não aceita acentos
    - [ ] Que a busca é mais lenta
    > Resposta Correta: É a distinção entre caracteres 'A' e 'a'.

4. Qual "Flag" (modificador) deve ser usada para tornar a busca case-insensitive?
    - [ ] Flag `g`
    - [x] Flag `i`
    - [ ] Flag `m`
    - [ ] Flag `s`
    > Resposta Correta: A flag `i` vem de "Ignore case".

5. Ao buscar "casa ", com um espaço no final, o Regex encontrará a palavra "casa" (sem espaço)?
    - [ ] Sim, ele ignora espaços extras
    - [x] Não, o espaço é considerado um caractere literal e deve estar presente
    - [ ] Depende da linguagem de programação
    - [ ] Apenas se for no final da linha
    > Resposta Correta: Espaços são caracteres literais em Regex.

6. O padrão "123" encontrará o número "123" em uma string como "ID_12345"?
    - [x] Sim, pois a sequência literal está contida na string
    - [ ] Não, ele só busca palavras completas
    - [ ] Apenas se for o início da string
    - [ ] Não, números não podem ser buscados literalmente
    > Resposta Correta: O match ocorre na parte da string que corresponde ao padrão.

7. Qual a diferença entre "CASA" (padrão) e "casa" (texto) sem flags?
    - [ ] São idênticos para o Regex
    - [x] O Regex não encontrará correspondência (No match)
    - [ ] O Regex encontrará apenas as letras "A"
    - [ ] O computador emitirá um alerta de erro
    > Resposta Correta: Sem a flag `i`, o padrão e o texto devem ter a mesma caixa.

8. Posso usar acentos em uma busca literal, como "maçã"?
    - [x] Sim, caracteres acentuados são tratados como caracteres literais normais
    - [ ] Não, Regex não suporta caracteres especiais da língua portuguesa
    - [ ] Sim, mas o Regex101 não mostra
    - [ ] Apenas se você converter para código ASCII
    > Resposta Correta: Acentos são suportados perfeitamente.

9. Se eu buscar por " " (dois espaços), o que o Regex encontrará?
    - [ ] Apenas uma quebra de linha
    - [ ] Nada, espaços não são pesquisáveis
    - [x] Exatamente duas ocorrências de espaços seguidos
    - [ ] Qualquer lugar onde falte um caractere
    > Resposta Correta: Espaços seguidos formam um padrão literal válido.

10. No Regex101, onde as "Flags" geralmente são configuradas?
    - [ ] No meio do texto de teste
    - [ ] Elas não existem no site
    - [x] No canto superior direito, ao lado da barra de expressão
    - [ ] No rodapé da página
    > Resposta Correta: Existe um ícone de bandeira ou um campo específico para flags (ex: `/padrão/gi`).