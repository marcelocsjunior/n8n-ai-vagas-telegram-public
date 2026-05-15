# n8n AI Vagas Telegram

Agente de vagas com n8n, IA local via Ollama, Google Drive, Google Sheets e Telegram.

## Objetivo

Automatizar a análise de aderência entre currículo e vagas, registrar resultados em planilha e enviar um resumo operacional pelo Telegram.

## Workflow overview

<img width="1670" height="376" alt="image" src="https://github.com/user-attachments/assets/c7bd7152-cbbe-4328-a882-4dc0388cf60d" />

## Fluxo principal

1. Schedule Trigger inicia a execução diária.
2. Google Drive baixa o currículo.
3. Google Sheets lê critérios de busca.
4. LinkedIn é consultado conforme os critérios.
5. O workflow extrai e normaliza os dados das vagas.
6. Ollama executa a análise via AI Agent.
7. Google Sheets registra logs.
8. Telegram recebe o resumo final.

## Stack

- n8n
- Ollama
- llama3.2:3b
- Google Drive
- Google Sheets
- Telegram Bot API
- Linux Server

## Workflow exportado

Arquivo sanitizado:

```text
workflows/agente-vagas-ia-local-telegram.json
```

O arquivo foi preparado para versionamento seguro. Identificadores reais, links privados e metadados sensíveis foram substituídos por placeholders.

Após importar no n8n, reconfigure as conexões externas e os IDs privados diretamente na sua instância local.

## Estrutura

```text
.
├── docs/
│   ├── configuration-example.md
│   ├── roadmap.md
│   ├── setup-google-service-account.md
│   ├── setup-n8n.md
│   ├── setup-ollama.md
│   └── setup-telegram.md
├── examples/
│   ├── sheet-aspiracao-example.csv
│   └── sheet-logs-example.csv
├── prompts/
│   └── ai-agent-prompt.md
├── workflows/
│   ├── README.md
│   └── agente-vagas-ia-local-telegram.json
├── .gitignore
├── CHANGELOG.md
├── README.md
└── SECURITY.md
```

## Segurança

Não versionar segredos, arquivos privados, currículo real, prints com dados sensíveis ou links privados.

## Status

- Google Drive: OK
- Google Sheets: OK
- Ollama: OK
- AI Agent: OK
- Telegram: OK
- Prompt definitivo: OK
- Workflow sanitizado no GitHub: OK
- Imagem do workflow no README: OK

## Funcionalidades entregues

- Download automatizado do currículo via Google Drive.
- Leitura de critérios de vaga no Google Sheets.
- Análise de aderência com IA local via Ollama.
- Registro estruturado de logs no Google Sheets.
- Envio automático do resumo final pelo Telegram.
