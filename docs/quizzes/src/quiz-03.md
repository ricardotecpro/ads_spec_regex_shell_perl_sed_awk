# Quiz 03 - Metacaracteres Fundamentais 🔣

1. O que o metacaractere ponto (`.`) representa?
    - [ ] O fim de uma frase
    - [x] Qualquer caractere único (exceto quebra de linha)
    - [ ] Apenas letras minúsculas
    - [ ] Apenas números
    > Resposta Correta: O ponto é o coringa universal para um único caractere.

2. Qual atalho representa "qualquer dígito numérico"?
    - [ ] `\w`
    - [ ] `\s`
    - [x] `\d`
    - [ ] `\t`
    > Resposta Correta: `\d` vem de "digit".

3. O que o atalho `\w` captura?
    - [ ] Apenas letras maiúsculas
    - [x] Letras, números e o caractere underline (`_`)
    - [ ] Apenas símbolos especiais
    - [ ] Somente espaços em branco
    > Resposta Correta: `\w` (word character) inclui alfanuméricos e `_`.

4. Qual a função da barra invertida (`\`) antes de um metacaractere?
    - [ ] Excluir o caractere da busca
    - [ ] Tornar a busca mais rápida
    - [x] Aplicar o "escape", buscando o caractere literal em vez do seu poder especial
    - [ ] Mudar a cor do texto no editor
    > Resposta Correta: O escape desativa o metacaractere (ex: `\.`).

5. Se eu usar o padrão `\s`, o que encontrarei?
    - [ ] Símbolos de dinheiro
    - [x] Espaços, tabulações e quebras de linha
    - [ ] Apenas a letra "s"
    - [ ] Somente o início da frase
    > Resposta Correta: `\s` captura "whitespace" (espaços em branco).

6. O que representa a letra maiúscula nos atalhos, como `\D`?
    - [ ] Uma busca mais forte
    - [x] A negação (qualquer coisa que NÃO seja um dígito)
    - [ ] Apenas letras em caixa alta
    - [ ] Um erro de sintaxe
    > Resposta Correta: Maiúsculas costumam negar o atalho original.

7. Para encontrar um endereço de IP como `127.0.0.1`, qual o Regex mais correto?
    - [ ] `127.0.0.1` (sem escape)
    - [x] `127\.0\.0\.1` (com escape)
    - [ ] `\d\d\d.\d.\d.\d`
    - [ ] `127*0*0*1`
    > Resposta Correta: O ponto real deve ser escapado para evitar que funcione como coringa.

8. O padrão `c.sa` dará match em "coisa"?
    - [ ] Sim, o ponto pega as letras "oi"
    - [x] Não, o ponto representa apenas UM caractere único
    - [ ] Sim, ele ignora o número de letras
    - [ ] Não, faltou o escape
    > Resposta Correta: Um ponto = um caractere. Para "oi" seriam necessários dois pontos.

9. Qual atalho captura o espaço entre duas palavras em "Olá Mundo"?
    - [ ] `\d`
    - [x] `\s`
    - [ ] `\w`
    - [ ] `.` (apenas se for o último recurso)
    > Resposta Correta: `\s` é o específico para espaços.

10. Como eu busco uma barra invertida literal (`\`) em um texto?
    - [ ] Digitando apenas `\`
    - [x] Digitando `\\` (escapando a própria barra)
    - [ ] Digitando `/`
    - [ ] Usando o ponto `.`
    > Resposta Correta: Como a barra é o caractere de escape, ela precisa escapar a si mesma.