# Setup n8n

## Objetivo

Documentar a configuração operacional do workflow no n8n.

## Workflow

Baseado no template público de análise de currículo contra vagas.

## Nodes principais

- Download file: baixa o currículo do Google Drive.
- Get row(s) in sheet: lê critérios na planilha.
- AI Agent: executa análise com IA local.
- Ollama Chat Model: modelo conectado ao AI Agent.
- Update Logs: grava resultado no Google Sheets.
- Send a text message: envia análise no Telegram.

## Ligação recomendada no estágio atual

```text
AI Agent -> Send a text message
```

## Observação operacional

Manter o node Parse AI Output desativado enquanto o retorno do modelo local não estiver padronizado em JSON confiável.
