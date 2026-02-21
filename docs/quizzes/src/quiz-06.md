# Quiz 06 - Âncoras ⚓

1. O que a âncora `^` representa (fora de colchetes)?
    - [ ] O fim da linha
    - [x] O início da linha ou do texto
    - [ ] Uma negação
    - [ ] Um caractere especial
    > Resposta Correta: O `^` ancora a busca no começo da linha.

2. Qual símbolo usamos para indicar o fim de uma linha?
    - [ ] `^`
    - [ ] `#`
    - [x] `$`
    - [ ] `&`
    > Resposta Correta: O cifrão `$` ancora a busca no final da linha.

3. Por que usamos `^` e `$` juntos em validação de formulários?
    - [ ] Para economizar memória
    - [x] Para garantir que o padrão preencha a linha inteira, sem extras
    - [ ] Para permitir qualquer caractere no meio
    - [ ] Para transformar o texto em maiúsculas
    > Resposta Correta: Garante que o input atenda exatamente à regra do início ao fim.

4. O padrão `^abc` encontrará a palavra "abc" em "123abc"?
    - [ ] Sim, ele ignora o início
    - [x] Não, pois "abc" não está no início da string
    - [ ] Sim, mas apenas se usar a flag global
    - [ ] Apenas em sistemas Windows
    > Resposta Correta: A busca falha porque o início da string é "1".

5. O padrão `xyz$` dará match no texto "arquivo_xyz.txt"?
    - [ ] Sim, contém xyz
    - [x] Não, pois a string termina com ".txt" e não com "xyz"
    - [ ] Sim, mas apenas o "xyz"
    - [ ] Depende do editor de texto
    > Resposta Correta: A âncora `$` exige que o padrão seja o último item.

6. Qual o efeito da flag `m` (multiline) nas âncoras?
    - [ ] Desativa as âncoras
    - [x] Faz com que `^` e `$` funcionem para CADA linha de um texto, e não apenas o texto todo
    - [ ] Permite buscar em múltiplos arquivos
    - [ ] Mudar o idioma do motor Regex
    > Resposta Correta: Trata cada quebra de linha como um novo início/fim.

7. O padrão `^\d{3}$` aceita o texto "1234"?
    - [ ] Sim, contém 3 dígitos
    - [x] Não, pois a linha inteira deve ter exatamente 3 dígitos
    - [ ] Sim, mas ignora o último número
    - [ ] Apenas se houver um espaço depois
    > Resposta Correta: O padrão exige 3 dígitos e o fim da linha logo após.

8. Se eu quiser encontrar uma linha vazia (sem nenhum caractere), qual o padrão?
    - [ ] ` ` (espaço)
    - [ ] `.*`
    - [x] `^$`
    - [ ] `\s`
    > Resposta Correta: Início seguido imediatamente pelo fim significa vazio.

9. O padrão `^$` daria match em um texto com um único espaço?
    - [ ] Sim
    - [x] Não, pois o espaço é um caractere e estaria entre o início e o fim
    - [ ] Apenas se for no Linux
    - [ ] Sim, pois espaço é invisível
    > Resposta Correta: O espaço impediria o match de `^$`.

10. No Regex, o símbolo `^` dentro de `[]` (como em `[^0-9]`) tem o mesmo sentido de âncora?
    - [ ] Sim, sempre
    - [x] Não, dentro de colchetes ele significa negação
    - [ ] Apenas se for a primeira letra
    - [ ] Sim, mas apenas em JavaScript
    > Resposta Correta: O contexto muda completamente o significado do símbolo.