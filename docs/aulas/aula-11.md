# Aula 11 – Regex com Python 🐍

Python é uma das linguagens mais poderosas para processamento de texto e dados. Para usar Regex, utilizamos a biblioteca padrão `re`.

---

## 📦 A Biblioteca `re`

Diferente do JavaScript, no Python os métodos de Regex fazem parte de um módulo que você precisa importar.

```python
import re

texto = "O ano é 2024"
```

### 1. `re.search(padrao, string)`
Procura a primeira ocorrência do padrão. Retorna um objeto de "Match" ou `None`.

```python
match = re.search(r"\d+", texto)
if match:
    print(f"Encontrado: {match.group()}") # "2024"
```

### 2. `re.findall(padrao, string)`
Retorna uma **lista** com todas as ocorrências encontradas.

```python
texto = "A1, B2, C3"
matches = re.findall(r"\d", texto)
print(matches) # ["1", "2", "3"]
```

### 3. `re.sub(padrao, substituto, string)`
Substitui as ocorrências por um novo texto (equivalente ao `.replace` do JS).

```python
limpo = re.sub(r"\s+", "_", "Texto com espaços")
print(limpo) # "Texto_com_espaços"
```

---

## 🏗️ O uso do `r""` (Raw Strings)

Em Python, sempre use o prefixo `r` antes das aspas do seu Regex. Isso evita que o Python interprete as barras invertidas `\` como comandos especiais dele mesmo.

- **Correto**: `re.search(r"\d", texto)`
- **Errado**: `re.search("\d", texto)` (pode causar bugs!)

---

## 💻 Exemplo em TermynalJS (Python CLI)

<div class="termy">
$ # Rodando script rápido em Python
$ python -c "import re; print(re.findall(r'\w+', 'Regex é top'))"
$ ['Regex', 'é', 'top']
$
$ # Verificando se começa com letra
$ python -c "import re; print(bool(re.match(r'[a-zA-Z]', '123')))"
$ False
</div>

---

## 📝 Exercícios de Fixação

1.  **Básico**: Importe a biblioteca `re` e verifique se a palavra "Python" existe na frase "Aprendendo Python com Regex".
2.  **Básico**: Use `findall()` para extrair todos os números de uma string: `"Pedidos #102, #305 e #400"`.
3.  **Intermediário**: Use `re.sub()` para remover todos os parênteses de um número de telefone: `(11) 9999-8888`.
4.  **Intermediário**: Crie um script que use `re.search()` para encontrar a primeira data no formato `DD/MM/AAAA`.
5.  **Desafio**: Crie uma função em Python que receba uma lista de e-mails e retorne apenas os que terminam em `@empresa.com`.

---

## 🚀 Mini-Projeto: Extrator de Links (Python)

**Objetivo**: Extrair todas as URLs de um bloco de texto.

1.  Código Sugerido:
    ```python
    import re
    
    html = 'Acesse <a href="http://google.com">Google</a> e <a href="https://python.org">Python</a>'
    links = re.findall(r'https?://[\w.]+', html)
    
    for link in links:
        print(f"Link encontrado: {link}")
    ```
2.  Desafio: Tente fazer o `findall` retornar apenas o domínio (sem o http).