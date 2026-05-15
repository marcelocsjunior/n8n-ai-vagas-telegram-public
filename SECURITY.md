# Security Policy

## Dados sensiveis

Este projeto pode envolver integracoes com Google, Telegram e dados pessoais de curriculo.

Nunca versionar:

- Chaves JSON de service account.
- Tokens de bot.
- Arquivos .env reais.
- Curriculos reais.
- Prints com credenciais.
- Links privados de arquivos.

## Antes de publicar o repositorio

1. Revisar historico de commits.
2. Verificar arquivos JSON exportados do n8n.
3. Remover credenciais embutidas.
4. Substituir dados reais por exemplos.
5. Validar que o workflow exportado usa placeholders.

## Recomendacao

Manter o repositorio privado enquanto houver dados reais ou configuracoes sensiveis no projeto.
