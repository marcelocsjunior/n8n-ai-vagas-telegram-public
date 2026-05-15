# Setup Google Service Account

## Objetivo

Permitir que o n8n acesse Google Drive e Google Sheets usando uma conta de serviço.

## Recursos usados

- Google Drive: download do currículo.
- Google Sheets: leitura de critérios e gravação de logs.

## Checklist

1. Criar conta de serviço no Google Cloud.
2. Gerar arquivo de autenticação no Google Cloud.
3. Criar credencial Google no n8n usando esse arquivo.
4. Compartilhar o arquivo do currículo com a conta de serviço.
5. Compartilhar a planilha com a conta de serviço.
6. Testar os nodes Google Drive e Google Sheets.

## Importante

Nunca versionar arquivos de autenticação no GitHub.

Esses arquivos devem ficar apenas no ambiente local ou servidor e fora do repositório.
