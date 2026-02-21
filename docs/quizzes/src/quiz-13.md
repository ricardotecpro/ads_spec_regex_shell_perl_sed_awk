# Quiz 13 - Extração de Dados ⛏️

1. Qual a principal diferença entre Validação e Extração?
    - [ ] Nenhuma, são sinônimos
    - [x] Validação verifica se o todo está correto; Extração isola partes específicas
    - [ ] Validação é mais lenta
    - [ ] Extração só funciona com nomes
    > Resposta Correta: Na extração, buscamos "matches" dentro de um texto maior.

2. Em Python, qual função usamos para extrair uma LISTA de todos os matches?
    - [ ] `re.search()`
    - [x] `re.findall()`
    - [ ] `re.extract()`
    - [ ] `re.sub()`
    > Resposta Correta: `findall` retorna todos os resultados em uma lista.

3. Qual a função da flag `-o` no comando `grep` do terminal?
    - [ ] Abrir o arquivo
    - [x] Mostrar apenas a parte do texto que deu match (only matching)
    - [ ] Ocultar o resultado
    - [ ] Ordenar os resultados
    > Resposta Correta: `-o` é fundamental para extrações rápidas no terminal.

4. O padrão `#[a-zA-Z\d_]+` é ideal para extrair:
    - [ ] E-mails
    - [x] Hashtags de redes sociais
    - [ ] Números de telefone
    - [ ] Links de sites
    > Resposta Correta: Ele busca o símbolo `#` seguido de caracteres alfanuméricos.

5. Ao usar parênteses em um padrão de extração, o que acontece no resultado do `match` ou `findall`?
    - [ ] O Regex dá erro
    - [x] Ele retorna apenas o conteúdo que estava dentro dos parênteses (Grupo de Captura)
    - [ ] Ele ignora os parênteses
    - [ ] Ele inverte o texto
    > Resposta Correta: Parênteses isolam o que você realmente quer extrair do resto do padrão.

6. Como extrair todos os anos (4 dígitos) de um texto longo?
    - [ ] `\d{4}`
    - [ ] `[0-9]{4}`
    - [x] Ambas as opções estão corretas
    - [ ] Nenhuma, precisa usar âncoras
    > Resposta Correta: Para extração, não usamos âncoras `^` e `$`, pois queremos encontrar no meio do texto.

7. No padrão `href="([^"]+)"`, o que o conjunto `[^"]+` faz?
    - [ ] Busca apenas aspas
    - [x] Captura tudo o que NÃO for aspas (garantindo que ele pare na aspas de fechamento)
    - [ ] Deleta o link
    - [ ] Busca apenas letras
    > Resposta Correta: É uma técnica comum para capturar conteúdo entre delimitadores.

8. Para extrair apenas o domínio de um e-mail (ex: `gmail.com`), qual o padrão correto?
    - [ ] `@.*`
    - [x] `@([\w.]+)`
    - [ ] `.*@`
    - [ ] `[a-z]+`
    > Resposta Correta: Captura tudo o que vem após o `@`.

9. O Regex `[A-Z]{2}` extrairá a sigla "SP" da frase "Moro em SP"?
    - [x] Sim
    - [ ] Não, falta a flag global
    - [ ] Apenas se "SP" estiver no final
    - [ ] Não, Regex só busca palavras de 3 letras
    > Resposta Correta: Siglas de 2 letras maiúsculas darão match perfeitamente.

10. Em uma busca por valores monetários `R\$ \d+`, o cifrão `$` precisa de escape?
    - [x] Sim, pois `$ sozinho` é a âncora de fim de linha
    - [ ] Não, o Regex entende pelo contexto
    - [ ] Sim, mas apenas se estiver no final
    - [ ] Não, pois é um símbolo de dinheiro
    > Resposta Correta: Metacaracteres devem ser escapados quando buscamos o símbolo literal.