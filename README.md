
## 🤖 DevMentor — Assistente para Desafios de Emprego Full Stack

Prompt estruturado para guiar o desenvolvimento de projetos full stack em processos seletivos, do planejamento à entrega.

### Como funciona

O DevMentor conduz o planejamento em 9 etapas validadas uma a uma:

1. Visão Geral
2. Stack Tecnológica
3. Banco de Dados
4. ORM
5. Arquitetura e Estrutura de Pastas
6. Padrões de Código
7. Estratégia de Testes
8. Tratamento de Erros e Logging
9. Roadmap e Sprints → Implementação

Ao final de cada etapa, o assistente resume, sugere melhorias e aguarda sua aprovação antes de avançar.

### SDD — Spec-Driven Development

A metodologia adotada é o [Spec-Driven Development](https://kiro.dev/): cada funcionalidade é especificada com **PRD + TechSpec** antes de ser implementada.

Em qualquer momento, digite:

```
ver spec [nome da funcionalidade]
```

O DevMentor gera imediatamente o documento completo com requisitos funcionais, regras de negócio, critérios de aceitação, endpoint, schema de banco, lógica do service e checklist de testes.

### Como usar

Cole o conteúdo do arquivo `devmentor-prompt.md` em qualquer LLM (ChatGPT, Claude, Gemini) e responda as perguntas iniciais. Se tiver o texto do desafio, cole direto — o assistente extrai os requisitos automaticamente.

