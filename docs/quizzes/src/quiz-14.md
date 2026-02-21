# Quiz 14 - Limpeza e Transformação 🧼

1. Qual o melhor uso do Regex no processo de sanitização de dados?
    - [ ] Criar novos bancos de dados
    - [x] Remover caracteres indesejados ou proibidos de um input
    - [ ] Traduzir o texto para outro idioma
    - [ ] Aumentar o tamanho das fontes
    > Resposta Correta: Regex é excelente para remover "lixo" (caracteres especiais, espaços extras) de entradas de usuários.

2. O padrão `\s{2,}` é usado para encontrar:
    - [ ] Pelo menos dois números
    - [x] Dois ou mais espaços em branco seguidos
    - [ ] Erros de ortografia
    - [ ] Palavras com duas letras
    > Resposta Correta: Ajuda a identificar e remover espaços duplos.

3. Como representamos a troca de posição entre dois grupos de captura na substituição?
    - [ ] `1$ 2$`
    - [x] `$2 $1` (ou \2 \1)
    - [ ] `swap(1,2)`
    - [ ] `{2}{1}`
    > Resposta Correta: A ordem dos identificadores de grupo define a nova ordem do texto.

4. O padrão `^\s+|\s+$` serve para:
    - [ ] Contar palavras
    - [x] Localizar espaços no início OU no fim do texto (Trim)
    - [ ] Validar e-mails
    - [ ] Deletar todo o texto
    > Resposta Correta: É a implementação manual do método "Trim" das linguagens.

5. Ao transformar `2024-10-21` para `21/10/2024`, o Regex original deve ter quantos grupos de captura?
    - [ ] 1
    - [ ] 2
    - [x] 3 (Ano, Mês, Dia)
    - [ ] Nenhum
    > Resposta Correta: Cada parte da data precisa ser isolada para ser reordenada.

6. O que o padrão `\D` faz em uma operação de limpeza de telefone?
    - [ ] Encontra apenas dígitos
    - [x] Encontra tudo o que NÃO é um dígito (parênteses, traços, espaços)
    - [ ] Exclui a linha inteira
    - [ ] Formata o número
    > Resposta Correta: Útil para extrair apenas os números brutos.

7. Qual a vantagem de usar Regex para converter nomes em "Slugs" de URL?
    - [ ] Deixa a URL colorida
    - [x] Automatiza a troca de caracteres especiais por hífens de forma padrão
    - [ ] Garante que o site suba no Google
    - [ ] Protege contra hackers
    > Resposta Correta: Padroniza o formato de links de forma eficiente.

8. No padrão `(<[^>]+>)`, o que estamos tentando encontrar?
    - [ ] Links de sites
    - [ ] Imagens
    - [x] Qualquer tag HTML (para remoção ou extração)
    - [ ] Comentários em Python
    > Resposta Correta: Busca o sinal de `<` seguido de qualquer coisa que não seja `>`, fechando em `>`.

9. O método de substituição é destrutivo ou gera uma nova string?
    - [ ] Destrói a string original para sempre
    - [x] Geralmente gera uma nova string transformada, mantendo a original intacta
    - [ ] Depende da cor do terminal
    - [ ] Só funciona se houver match
    > Resposta Correta: Strings costumam ser imutáveis; a função retorna o resultado da transformação.

10. Posso usar Regex para remover comentários de um código-fonte?
    - [x] Sim, identificando padrões como `//` ou `/* */`
    - [ ] Não, Regex não lê código
    - [ ] Apenas se o código estiver em JavaScript
    - [ ] Sim, mas isso apagará todo o programa
    > Resposta Correta: É um uso clássico para limpeza de arquivos de configuração ou código.