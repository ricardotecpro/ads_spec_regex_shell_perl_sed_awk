# Quiz 09 - Modificadores (Flags) 🚩

1. O que são as Flags em Regex?
    - [ ] Símbolos usados dentro da expressão
    - [x] Modificadores que mudam o comportamento global da execução
    - [ ] Atalhos para números
    - [ ] Erros de sintaxe
    > Resposta Correta: Elas definem COMO a expressão deve ser processada.

2. Qual a função da flag `i`?
    - [ ] Inserir texto
    - [ ] Inverter a busca
    - [x] Ignorar a diferença entre maiúsculas e minúsculas
    - [ ] Identificar números
    > Resposta Correta: "i" vem de case-insensitive.

3. Sem a flag `g` (global), o que acontece em um texto com várias ocorrências de um padrão?
    - [ ] O Regex encontra todas
    - [x] O Regex para após encontrar a primeira ocorrência
    - [ ] O Regex dá erro
    - [ ] O Regex encontra apenas a última
    > Resposta Correta: O comportamento padrão é parar no primeiro match.

4. Para que serve a flag `m` (multiline)?
    - [ ] Para buscar em vários arquivos ao mesmo tempo
    - [x] Para que `^` e `$` considerem cada linha individualmente
    - [ ] Para permitir mais de um Regex na mesma linha
    - [ ] Para formatar o texto em colunas
    > Resposta Correta: Muda o comportamento das âncoras de início e fim.

5. O que a flag `s` (DotAll) permite ao metacaractere ponto (`.`)?
    - [ ] Ser mais rápido
    - [x] Dar match em quebras de linha (`\n`)
    - [ ] Ser ignorado
    - [ ] Só encontrar espaços
    > Resposta Correta: Normalmente o `.` ignora o caractere de nova linha.

6. Onde as flags costumam ser posicionadas na sintaxe padrão?
    - [ ] No início: `gi/padrao/`
    - [x] No final: `/padrao/gi`
    - [ ] No meio: `/pad/gi/rao`
    - [ ] Dentro dos colchetes
    > Resposta Correta: Elas vêm logo após o delimitador final.

7. Qual flag é essencial para um comando de "Substituir Tudo" em um editor?
    - [ ] Flag `i`
    - [x] Flag `g`
    - [ ] Flag `m`
    - [ ] Flag `s`
    > Resposta Correta: Sem a flag global, apenas o primeiro item seria substituído.

8. Se eu usar `/abc/i`, ele encontrará "ABC"?
    - [x] Sim, devido à flag de ignore case
    - [ ] Não, falta a flag global
    - [ ] Apenas se o texto estiver entre aspas
    - [ ] Somente em JavaScript
    > Resposta Correta: A flag `i` resolve a diferença de caixa.

9. A flag `u` (Unicode) é importante para:
    - [ ] Deixar o código mais bonito
    - [x] Processar corretamente caracteres especiais, emojis e símbolos complexos
    - [ ] Traduzir o texto
    - [ ] Aumentar o tamanho do arquivo
    > Resposta Correta: Garante o tratamento correto de caracteres multi-byte.

10. Posso combinar várias flags juntas, como `gim`?
    - [x] Sim, elas se somam e aplicam todos os comportamentos ao mesmo tempo
    - [ ] Não, deve-se usar apenas uma por vez
    - [ ] Sim, mas a ordem altera o resultado
    - [ ] Apenas em ferramentas de terminal
    > Resposta Correta: As flags podem ser combinadas livremente.