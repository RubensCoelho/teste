# Projeto Teste

Projeto de teste para exploração e configuração do **Claude Code** com integração ao **VS Code**, utilizando hooks de contexto e servidores MCP.

## Estrutura do Projeto

```
Projeto Teste/
├── .github/
│   └── hooks/
│       └── context-mode.json   # Hooks do Claude Code (PreToolUse, PostToolUse, SessionStart)
├── .vscode/
│   └── mcp.json                # Configuração do servidor MCP (context-mode)
└── Teste/                      # Diretório principal do projeto
```

## Configurações

### Hooks do Claude Code

O arquivo `.github/hooks/context-mode.json` configura os seguintes hooks integrados ao VS Code Copilot:

- **PreToolUse** — executado antes de cada uso de ferramenta
- **PostToolUse** — executado após cada uso de ferramenta
- **SessionStart** — executado no início de cada sessão

### Servidor MCP

O arquivo `.vscode/mcp.json` configura o servidor MCP `context-mode`, que gerencia o contexto das sessões do Claude Code dentro do VS Code.

## Requisitos

- [Claude Code](https://claude.ai/code)
- [VS Code](https://code.visualstudio.com/)
- `context-mode` instalado e disponível no PATH

## Como usar

1. Clone o repositório:
   ```bash
   git clone https://github.com/RubensCoelho/teste.git
   ```

2. Abra o projeto no VS Code:
   ```bash
   code "Projeto Teste"
   ```

3. Inicie uma sessão do Claude Code — os hooks e o servidor MCP serão ativados automaticamente.
