# Aula 14 – Limpeza e Transformação 🧼

Muitas vezes recebemos dados "sujos": com espaços extras, formatos inconsistentes ou informações desnecessárias. O Regex é o "sabão" ideal para limpar esses dados.

---

## 🧹 Removendo Espaços Extras

Espaços em branco antes, depois ou duplos no meio do texto são vilões de bancos de dados.

- **Espaços no início/fim**: `^\s+|\s+$`
- **Espaços duplos**: `\s{2,}` (substituir por um único espaço `" "`).

---

## 🔄 Transformando Formatos (Reordenação)

Usando grupos de captura, podemos mudar a ordem das informações.

- **Transformar**: `2024-10-21` (ISO) -> `21/10/2024` (BR)
- **Regex**: `(\d{4})-(\d{2})-(\d{2})`
- **Substituição**: `$3/$2/$1`

---

## 🎭 Mascarando Dados Sensíveis

Esconder partes de um código ou e-mail por segurança.

- **Texto**: `123.456.789-00`
- **Regex**: `\d(?=\d{2})` (Usa um *lookahead* para pegar todos os números exceto os dois últimos).
- **Substituição**: `*`
- **Resultado**: `***.***.***-00`

---

## 📊 Fluxo de Transformação

```mermaid
graph LR
    Input["Dado Sujo"] --> Find["Padrão Regex"]
    Find --> Replace["Ação: Reorder / Delete / Replace"]
    Replace --> Output["Dado Pronto"]
```

---

## 💻 Exemplo em TermynalJS (JS Replace)

<div class="termy">
$ # Removendo tags HTML de um texto
$ node -e "console.log('<p>Olá</p>'.replace(/<[^>]+>/g, ''))"
$ Olá
$
$ # Limpando caracteres não-numéricos de um telefone
$ node -e "console.log('(11) 9999-8888'.replace(/\D/g, ''))"
$ 1199998888
</div>

---

## 📝 Exercícios de Fixação

1.  **Básico**: Crie um Regex para remover todos os parênteses e traços de um CPF.
2.  **Básico**: Use `.replace()` para trocar todas as letras "a" por "@" em uma frase.
3.  **Intermediário**: Dado um nome completo `"Pires, Ricardo"`, use Regex para transformá-lo em `"Ricardo Pires"`. (Dica: Use dois grupos e troque sua ordem).
4.  **Intermediário**: Crie um padrão que remova todas as quebras de linha duplas, transformando-as em apenas uma.
5.  **Desafio**: No Regex101, use a aba "Substitution" para transformar uma lista de preços no formato `150.00` para o formato brasileiro `150,00` usando grupos.

---

## 🚀 Mini-Projeto: Sanitizador de Inputs

**Objetivo**: Criar uma função que "limpe" um nome de usuário, removendo qualquer caractere que não seja uma letra ou número.

1.  Código Sugerido (JS):
    ```javascript
    function limparUsuario(input) {
        return input.replace(/[^a-zA-Z0-9]/g, "");
    }
    
    console.log(limparUsuario("ricardo! @pires 101")); // "ricardopires101"
    ```
2.  Desafio: Modifique a função para que ela também converta tudo para minúsculas após a limpeza.