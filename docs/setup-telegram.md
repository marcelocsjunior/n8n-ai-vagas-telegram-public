# Setup Telegram

## Objetivo

Enviar a análise final do AI Agent para um usuário no Telegram.

## Node n8n

```text
Resource: Message
Operation: Send Message
```

## Texto inicial para teste

```text
Teste n8n Telegram OK
```

## Texto operacional inicial

```text
Agente de Vagas IA

Analise concluida:

{{$json.output}}
```

## Diagnóstico

Se a mensagem chegar vazia, verificar o output do node AI Agent e testar os campos:

```text
{{$json.output}}
{{$json.text}}
{{$json.response}}
```

## Erros comuns

### 403 Forbidden

O bot pode estar tentando enviar mensagem para outro bot ou para um chat incorreto.

### Chat not found

O usuário ainda pode não ter iniciado conversa com o bot, ou o Chat ID está incorreto.
