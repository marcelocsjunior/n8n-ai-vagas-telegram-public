# Changelog

Todas as mudanças relevantes deste projeto serão documentadas neste arquivo.

## [0.1.0] - 2026-05-15

### Adicionado

- Workflow n8n sanitizado para versionamento seguro.
- Integração com Google Drive para baixar currículo.
- Integração com Google Sheets para leitura de critérios e registro de logs.
- Processamento de vagas do LinkedIn com limite por execução.
- Análise de aderência usando IA local via Ollama.
- Modelo local configurado como `llama3.2:3b`.
- Envio da análise final via Telegram.
- Prompt operacional do AI Agent em português do Brasil.
- Documentação inicial de setup e segurança.
- Exemplos de abas Google Sheets.
- README com visão geral do workflow.

### Alterado

- OpenAI API removida do desenho operacional por custo.
- Parse AI Output mantido fora do fluxo principal por instabilidade de JSON em modelo local.
- Export do workflow configurado com `active: false` para importação segura.

### Segurança

- IDs reais, dados privados, credenciais, URLs privadas e metadados sensíveis removidos do workflow versionado.
- Credenciais marcadas para reconfiguração manual no n8n após importação.
