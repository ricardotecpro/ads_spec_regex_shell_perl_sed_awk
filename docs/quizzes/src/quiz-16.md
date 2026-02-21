# Quiz 16 - Revisão Geral e Projeto Final 🏆

1. Qual o primeiro passo recomendado ao receber uma tarefa complexa de Regex?
    - [ ] Começar a digitar código imediatamente
    - [x] Testar o padrão e os dados de exemplo em uma ferramenta como Regex101
    - [ ] Pedir para outra pessoa fazer
    - [ ] Desistir e usar busca manual
    > Resposta Correta: Ferramentas de teste visual economizam muito tempo de depuração.

2. O que aprendemos sobre a normalização de datas em Regex?
    - [ ] É impossível fazer com Regex
    - [ ] Datas não devem ter separadores
    - [x] Podemos usar grupos de captura para reordenar Dia, Mês e Ano
    - [ ] Regex só aceita o formato americano
    > Resposta Correta: Grupos e substituição são perfeitos para mudar formatos.

3. Para normalizar "Pago", "pago" e "PAGO" em um único padrão, qual a melhor estratégia?
    - [ ] Escrever as três opções separadas por `|`
    - [x] Usar a palavra `pago` com a flag `i` (ignore case)
    - [ ] Usar o ponto `.`
    - [ ] Não há como fazer
    > Resposta Correta: A flag `i` simplifica muito a busca por palavras com variação de caixa.

4. Se o seu projeto final precisa extrair IPs, qual classe de caractere é a mais adequada?
    - [ ] `\w`
    - [x] `\d` (pois IPs são compostos por dígitos e pontos)
    - [ ] `\s`
    - [ ] `\A`
    > Resposta Correta: `\d` ou `[0-9]` são essenciais para encontrar números.

5. Em um script de limpeza, por que limpamos caracteres não-numéricos antes de salvar no banco?
    - [ ] Para o banco ficar mais bonito
    - [x] Para garantir integridade dos dados e facilitar cálculos futuros
    - [ ] Para o arquivo pesar mais
    - [ ] É apenas uma tradição
    > Resposta Correta: Dados limpos e padronizados evitam erros de processamento e lógica.

6. Qual metacaractere foi o mais versátil ao longo do curso para buscas rápidas?
    - [ ] `$`
    - [ ] `^`
    - [x] `.` (Ponto)
    - [ ] `\`
    > Resposta Correta: O ponto é o coringa para qualquer caractere único.

7. No seu projeto final, se você quiser garantir que o Regex pegue o nome de usuário até o símbolo `|`, o que deve usar?
    - [ ] `.*|`
    - [x] `.*?\|` (Preguiçoso com escape da barra)
    - [ ] `.+`
    - [ ] `^$`
    > Resposta Correta: O modo preguiçoso evita que o Regex pegue mais do que o necessário.

8. O que significa "Refatorar um Regex"?
    - [ ] Apagar e começar do zero
    - [x] Melhorar o padrão existente para torná-lo mais legível ou performático
    - [ ] Mudar a linguagem de programação
    - [ ] Adicionar mais erros
    > Resposta Correta: Refatoração foca em qualidade e eficiência.

9. Após terminar este curso, você se sente apto a:
    - [ ] Hackear a NASA
    - [x] Enfrentar desafios de manipulação e validação de texto com confiança
    - [ ] Criar uma nova linguagem de programação
    - [ ] Parar de usar computador
    > Resposta Correta: O objetivo foi dar autonomia e ferramentas para lidar com dados de texto.

10. Qual a mensagem final do curso sobre Expressões Regulares?
    - [ ] Elas são inúteis
    - [ ] Devem ser evitadas a todo custo
    - [x] São um superpoder que, se usado com sabedoria e boas práticas, aumenta muito a produtividade
    - [ ] São apenas para quem gosta de matemática
    > Resposta Correta: Regex é uma ferramenta essencial e poderosa no arsenal de qualquer profissional de TI.