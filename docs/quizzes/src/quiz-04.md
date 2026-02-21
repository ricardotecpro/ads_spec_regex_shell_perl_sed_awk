# Quiz 04 - Conjuntos de Caracteres 📦

1. Para que servem os colchetes `[]` em Regex?
    - [ ] Para indicar um comentário
    - [x] Para definir um conjunto de caracteres permitidos em uma posição
    - [ ] Para agrupar expressões complexas
    - [ ] Para marcar o início do texto
    > Resposta Correta: Os colchetes permitem escolher UM entre vários caracteres listados.

2. O padrão `[aeiou]` encontrará qual destes?
    - [ ] A palavra "aeiou" inteira
    - [x] Qualquer vogal individual minúscula
    - [ ] Apenas a letra "a"
    - [ ] Qualquer letra do alfabeto
    > Resposta Correta: Encontrará 'a', 'e', 'i', 'o' ou 'u' individualmente.

3. Como representamos o intervalo de todas as letras minúsculas de forma curta?
    - [ ] `[a,z]`
    - [ ] `[a..z]`
    - [x] `[a-z]`
    - [ ] `[a:z]`
    > Resposta Correta: O hífen `-` define o intervalo (range).

4. O que o conjunto `[0-9]` representa?
    - [ ] Apenas os números 0 e 9
    - [x] Qualquer algarismo de 0 a 9 (o mesmo que \d)
    - [ ] O resultado de uma conta de subtração
    - [ ] Uma data
    > Resposta Correta: Representa a classe dos dígitos decimais.

5. Qual símbolo é usado para NEGAR um conjunto quando colocado no início dos colchetes?
    - [ ] `!`
    - [ ] `-`
    - [x] `^`
    - [ ] `*`
    > Resposta Correta: O circunflexo no início nega o conjunto (ex: `[^...]`).

6. O padrão `[a-zA-Z]` encontrará qual tipo de caractere?
    - [ ] Apenas letras com acento
    - [x] Qualquer letra latina, seja maiúscula ou minúscula
    - [ ] Apenas as letras 'a' e 'z'
    - [ ] Letras e números misturados
    > Resposta Correta: Combina dois intervalos de letras.

7. Se eu usar `[^0-9]`, o que terei como resultado?
    - [ ] Apenas números negativos
    - [x] Qualquer caractere que NÃO seja um número
    - [ ] O número 0 e o número 9
    - [ ] Um erro de código
    > Resposta Correta: É a negação dos dígitos.

8. O conjunto `[123]` é diferente de `[1-3]`?
    - [ ] Sim, o primeiro busca o número 123
    - [x] Não, ambos buscam individualmente os números 1, 2 ou 3
    - [ ] Sim, o segundo é mais lento
    - [ ] Sim, o primeiro só aceita o número 1
    > Resposta Correta: Ambos representam os mesmos caracteres individuais.

9. Onde o hífen `-` deve ser colocado se eu quiser pesquisá-lo literalmente dentro de um conjunto sem que ele crie um intervalo?
    - [ ] No meio das letras
    - [x] No início ou no fim do conjunto (ex: `[-az]` ou `[az-]`)
    - [ ] Sempre fora dos colchetes
    - [ ] Ele não pode ser pesquisado em conjuntos
    > Resposta Correta: Nas extremidades ele perde o poder de definir intervalo.

10. O padrão `[A-Z][0-9]` daria match em qual destes textos?
    - [ ] a1
    - [x] B3
    - [ ] 9Z
    - [ ] AB
    > Resposta Correta: Primeiro caractere Maiúscula, segundo um Número.