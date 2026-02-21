# Quiz 15 - Desempenho e Boas Práticas ⚡

1. O que é o "Catastrophic Backtracking"?
    - [ ] Um erro de digitação
    - [x] Um estado onde o motor Regex tenta bilhões de combinações, travando o sistema
    - [ ] Quando o Regex volta para o início do arquivo
    - [ ] Uma flag de segurança
    > Resposta Correta: Ocorre em padrões complexos (geralmente quantificadores aninhados).

2. Qual destes padrões é considerado perigoso para a performance?
    - [ ] `[a-z]+`
    - [ ] `^\d+$`
    - [x] `(a+)+b`
    - [ ] `\s?`
    > Resposta Correta: O aninhamento de `+` dentro de outro `+` cria uma explosão combinatória.

3. Por que usar `(?:...)` em vez de `(...)`?
    - [ ] É mais bonito
    - [x] Melhora a performance ao evitar que o motor salve o match na memória (não-captura)
    - [ ] É a única forma de usar o OU `|`
    - [ ] Não há diferença real
    > Resposta Correta: Grupos de não-captura são mais leves para o sistema.

4. Em termos de performance, o que é melhor: `.*` ou `[0-9]+`?
    - [ ] `.*`, pois é o mais versátil
    - [x] `[0-9]+`, pois é mais específico e evita buscas desnecessárias
    - [ ] Dão no mesmo
    - [ ] Nenhum, use apenas letras
    > Resposta Correta: Quanto mais específico for o padrão, menos o motor precisa "adivinhar".

5. Para que servem as ferramentas de "Debugger" no Regex101?
    - [ ] Para traduzir o Regex
    - [x] Para ver passo a passo como o motor está tentando encontrar o match e onde ele falha
    - [ ] Para salvar o Regex na nuvem
    - [ ] Para criar gráficos coloridos
    > Resposta Correta: Essencial para identificar gargalos de performance.

6. O que significa "ReDoS"?
    - [ ] Redo Operation Software
    - [x] Regular Expression Denial of Service (Ataque de negação de serviço via Regex)
    - [ ] Regex Data System
    - [ ] Registro de Dados Online
    > Resposta Correta: É um ataque que explora Regex lentos para derrubar servidores.

7. Por que devemos usar âncoras (`^` e `$`) sempre que possível?
    - [ ] Para deixar o padrão mais longo
    - [x] Para limitar o espaço de busca e permitir que o motor falhe rápido se o início não bater
    - [ ] Porque é uma regra obrigatória do JavaScript
    - [ ] Para mudar o idioma da busca
    > Resposta Correta: Âncoras reduzem drasticamente o número de tentativas do motor.

8. Qual a melhor prática para lidar com expressões muito complexas e longas?
    - [ ] Escrever tudo em uma única linha gigante
    - [x] Comentar o código e, se a linguagem permitir, usar o modo "verbose" (com espaços e comentários)
    - [ ] Evitar usar Regex e fazer tudo com `if/else`
    - [ ] Usar apenas letras minúsculas
    > Resposta Correta: Documentação é vital para a manutenção do código.

9. Na alternância `A|B|C`, onde deve ficar o padrão mais frequente?
    - [ ] No final
    - [ ] No meio
    - [x] No início (da esquerda para a direita)
    - [ ] Não importa a ordem
    > Resposta Correta: O motor para no primeiro match satisfatório; colocar o comum primeiro economiza tempo.

10. Usar Regex é sempre a solução mais rápida para qualquer problema de string?
    - [ ] Sim, Regex é imbatível
    - [x] Não, para buscas muito simples (tipo `indexOf` ou `startsWith`), métodos nativos de string são mais rápidos
    - [ ] Apenas em Python
    - [ ] Sim, mas apenas no Linux
    > Resposta Correta: Use a ferramenta certa para o trabalho. Regex tem um custo de "compilação" inicial.