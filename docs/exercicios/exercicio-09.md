# Exercícios: Aula 09 – Modificadores (Flags) 🚩

Aprendendo a controlar o comportamento global do motor Regex.

---

## 🟢 Nível Básico

### 1. Ignorando a Caixa
Texto: `Maçã, maçã, MAÇÃ`

- **Tarefa**: Use o padrão `maçã` com a flag `i` para encontrar todas as variações.

### 2. Match Global
Texto: `um peixe, dois peixes, três peixes`

- **Tarefa**: Busque pela palavra `peixe` sem a flag `g` e depois com ela. Qual a diferença no número de matches?

---

## 🟡 Nível Intermediário

### 3. Ponto Total (DotAll)
Texto:
```text
Início do parágrafo.
Continuação na linha de baixo.
```

- **Tarefa**: Crie um padrão que tente capturar tudo o que começa em "Início" e termina em "baixo". 
- **Desafio**: Funciona sem a flag `s`? Por que o ponto `.` precisa dela aqui?

### 4. Multiline vs Global
Texto:
```text
# Título 1
# Título 2
Conteúdo
```

- **Tarefa**: Use `^#` com as flags `g` e `m` para encontrar todos os títulos que começam com `#`. O que acontece se remover a flag `m`?

---

## 🔴 Nível Desafio

### 5. Combinação Poderosa
Utilize o [Regex101](https://regex101.com/).

- **Tarefa**: Crie um Regex que localize links `http` ou `https` em um texto com várias linhas, ignorando se o protocolo está em maiúscula ou minúscula.
- **Dica**: Use as flags `/gi/`.