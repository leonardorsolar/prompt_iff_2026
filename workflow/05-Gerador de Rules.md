# Gerador de Rules Document para IDEs com IA

Cole o prompt abaixo no chat de qualquer IA (Claude, ChatGPT, Copilot Chat etc.).
Ela vai perguntar a ferramenta, analisar seu código e gerar o arquivo completo pronto para salvar.

---

## Prompt

cole daqui
```
Você é um especialista em configuração de ambientes de desenvolvimento com IA.

Vou criar o documento de rules do meu projeto. Antes de gerar, faça as seguintes perguntas, uma de cada vez:

**Pergunta 1:** Qual ferramenta você está usando?
- Cursor → arquivo: `.cursorrules` (raiz do projeto)
- Windsurf → arquivo: `.windsurfrules` (raiz do projeto)
- GitHub Copilot (VS Code) → arquivo: `.github/copilot-instructions.md` (raiz do repositório)
- Claude.ai → Project Instructions (configurações do Project)
- Outra → me informe o nome e eu identifico o formato correto

**Pergunta 2:** Posso analisar o seu código para gerar a rules?
O Cursor Rules é um sistema de instruções persistentes que você configura na sua ide/cli para guiar o comportamento do AI em um projeto específico.
Responda sim que farei a análise completa e preencherei todos os dados automaticamente para gerar o documento.

---

Após receber as respostas, analise o código fornecido e gere o documento completo com:

1. Identidade e papel da IA no projeto
2. Stack tecnológica e versões detectadas
3. Estrutura de pastas e organização do projeto
4. Padrões de código (nomenclatura, formatação, arquitetura)
5. Boas práticas obrigatórias (testes, tratamento de erros, segurança)
6. O que a IA NUNCA deve fazer neste projeto
7. Estilo de resposta esperado (tamanho, formato, idioma)
8. Exemplos dos padrões encontrados no próprio código

O documento deve estar pronto para ser copiado e salvo no caminho correto da ferramenta escolhida.
```
até aqui

---

## Referência rápida — onde salvar cada arquivo

| Ferramenta | Arquivo | Local |
|---|---|---|
| Cursor | `.cursorrules` | Raiz do projeto |
| Cursor (moderno) | `.cursor/rules/*.mdc` | Raiz do projeto |
| Windsurf | `.windsurfrules` | Raiz do projeto |
| Windsurf (moderno) | `.windsurf/rules/*.md` | Raiz do projeto |
| Copilot (VS Code) | `.github/copilot-instructions.md` | Raiz do repositório |
| Claude.ai | Project Instructions | Configurações do Project |