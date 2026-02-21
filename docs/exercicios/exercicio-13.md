# Exercícios: Aula 13 – Extração de Dados ⛏️

Praticando a captura seletiva de informações em textos complexos.

---

## 🟢 Nível Básico

### 1. Pegando Números de uma String
Texto: `O pedido #123 foi faturado por R$ 450.`

- **Tarefa**: Extraia todos os números (separadamente) desse texto.

### 2. Buscando Menções
Texto: `Fale com @ricardo ou @ana sobre o projeto.`

- **Tarefa**: Crie um Regex para extrair todas as menções que começam com `@`.

---

## 🟡 Nível Intermediário

### 3. Extraindo apenas o Domínio
Texto: `Links úteis: https://google.com, http://github.io, https://regex101.com`

- **Tarefa**: Use um grupo de captura para extrair apenas o domínio (ex: `google.com`), sem o protocolo `https://`.

### 4. Localizando IDs de Produtos
Texto: `Produtos: [ID:101], [ID:202], [ID:303]`

- **Tarefa**: Extraia apenas os números dos IDs que estão dentro dos colchetes.

---

## 🔴 Nível Desafio

### 5. Crawler de Imagens
Texto: `<img src="foto1.jpg"> <img src="banners/logo.png"> <img src="https://site.com/avatar.gif">`

- **Tarefa**: Crie um Regex que extraia apenas o caminho da imagem (o conteúdo dentro de `src="..."`).
- **Desafio Extra**: No seu teste, ele deve capturar `foto1.jpg`, `banners/logo.png` e a URL completa do avatar.