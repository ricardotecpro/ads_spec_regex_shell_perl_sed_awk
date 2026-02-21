# Projeto Final: Automatizador de Auditoria de Dados 🚀

Chegou a hora de provar suas habilidades! Neste projeto, você criará um script de limpeza de dados que transforma um arquivo de logs bagunçado em um relatório estruturado.

---

## 📁 O Arquivo de Entrada (`dados_brutos.txt`)

Imagine que você recebeu os seguintes registros:

```text
USER: ricardo123 | LOGIN: 21-10-2024 10:00 | IP: 192.168.0.1 | STATUS: success
USER: ana_f | LOGIN: 2024/10/21 10:05:30 | IP: 10.0.0.5 | STATUS: error
USER: joao.silva | LOGIN: 21.10.2024 (10:10) | IP: 172.16.254.1 | STATUS: SUCCESS
```

---

## 📋 Objetivos do Projeto

Seu script (Python ou JS) deve usar Regex para:

1.  **Extrair todos os nomes de usuários**.
2.  **Normalizar as Datas**: Transformar todos os formatos de data (`-`, `/`, `.`) e remover os parênteses do horário se houver.
3.  **Identificar o Status**: Contar quantos `SUCCESS` e quantos `ERROR` ocorreram, ignorando a caixa das letras.
4.  **Extrair os IPs**: Criar uma lista com todos os endereços IP encontrados.

---

## 💡 Dicas de Implementação

- Use `re.findall()` em Python para as listas.
- Use `re.sub()` ou `.replace()` para as normalizações de data.
- Use a flag `i` para o status.

---

## 📤 O que deve ser entregue (Simulado)

Um documento ou script que mostre:
- O Regex usado para cada item.
- O resultado final estruturado.

### Exemplo de Resultado Final:
```text
RELATÓRIO DE AUDITORIA
----------------------
Usuários: [ricardo123, ana_f, joao.silva]
Total Sucessos: 2
Total Erros: 1
IPs Bloqueados: [192.168.0.1, 10.0.0.5, 172.16.254.1]
```

---

## 🌟 Desafio Extra

Tente criar um Regex único que separe cada linha em 4 grupos de captura: `Usuário`, `Data`, `IP` e `Status`.

**Boa sorte, mestre do Regex!**