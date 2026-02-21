# Exercícios: Aula 05 – Quantificadores 🔢

Praticando a repetição de padrões e o comportamento guloso vs. preguiçoso.

---

## 🟢 Nível Básico

### 1. O Poder do +
Texto: `aaaaa bbb c dddddddd`

- **Tarefa**: Use `a+` para pegar todos os 'a's de uma vez só em um único match. Faça o mesmo para as outras letras.

### 2. Opcionais
Texto: `O arquivo pode ser foto.jpg ou imagem.jpeg.`

- **Tarefa**: Crie um padrão para capturar a extensão, onde o 'e' de `jpeg` seja opcional. (Dica: Use `jpe?g`).

---

## 🟡 Nível Intermediário

### 3. Quantidade Exata
Texto: `Código: 123456 | Serial: AB9876`

- **Tarefa**: Use `\d{6}` para encontrar apenas o código numérico de 6 dígitos.

### 4. Intervalos de Repetição
Texto: `O nome do usuário deve ter de 3 a 5 letras.`

- **Tarefa**: Crie um padrão que valide palavras compostas apenas por letras (`\w` ou `[a-z]`) que tenham entre 3 e 5 caracteres.

---

## 🔴 Nível Desafio

### 5. Fugindo da "Gulodice"
Texto: `O link é <a href="http://google.com">Google</a> e o outro é <a href="http://bing.com">Bing</a>.`

- **Tarefa**: Crie um padrão para capturar o conteúdo dentro de `href="..."`.
- **Desafio**: Tente usar `href=".*"` primeiro e veja o erro (ele pegará até o final da linha). Depois, use o quantificador preguiçoso `href=".*?"` para corrigir.